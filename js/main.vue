new Vue({
  el: '#app',
  data () {
    return {
      info: null,
      loading: true,
      errored: false,
        }
    },
filters: {
  titleLimit: function (text) {
    if (!text) return 'no title'
        if(text.length > 200)
            text = text.substring(0,200);
      return text;
  },
    dateFormat: function (date) {
    return moment(date).format('Do MMMM YYYY');
  },
    hyphenRemover: function(text){
       let str = text.replace(/-/g, ' ');
        return str;
    }
},
  mounted () {
    axios
      .get('https://api.tradeteq.com/marketplace/v2.5/story/how-will-investors-leverage-trade-finance-growth')
      .then(response => {
        this.info = response.data;
                this.details = this.info.value.copy;

                for (let j = 0; j < this.details.length; j++) {
                    this.str = this.details[j];
                    this.details[j]= this.str.split('\",'); 
                    this.details[j] = this.str.replace(/[\[\]']+/g, '');
                }          
      })
      .catch(error => {
        console.log(error)
        this.errored = true
      })
      .finally(() => this.loading = false)
  }
      
})

