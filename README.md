**Front end task - User Story**

**Tools:**

This task has been developed with Brackets Editor.

The techonologies i used for this task are:

- HTML/5
- CSS3
- Vuejs

and external libraries:

- Bootstrap CSS (for stylish)
- moment (formatting the date)
- axios (interacting/requesting with/from the api)
- Vuejs (used as the main interaction with the app)

**Run**

To run the webpage first you have to unzip the parent directory and then to run the index page on your favourite(popular) web browser. No web server installation or configuration is need for this task.

**Story**

First, read all the requirements from the code test.rtf. and writing down what’s the possible issue might be expect. After Understanding all the story page and asked any possible question, choose the right tools for the development.

Framework or Vanillia? 

Personally, i chose **vuejs** as i’m more experienced than any other front end js framework(react, angular) and i prefer it from the vanilla js for this task. The reason is that is easy readable, maintainable and safer than the pure js. Also i used the **axios** for the api request and **moment** for the same reason.

My assumption is to keep it as more minified as i can. For that reason, i’m using only one file for VueJs (without splitting it into external templates / components), css and root.

Why Bootstrap?

I used bootstrap for rapid development. In addition is giving some more general rules to have a consistent layout. However, custom css rules has been applied for the extra features.

__

To begin the development, an api call needs to be done to show what kind of data are going to be used. Typically an access to the link with the web browser should be ok.

Moving forward, scaffolding/creating the development environment with the necessary files and folders such as (index.html, main.css, main.vue, css, js). 

On the development, first establish access to the public tradeteq api by requesting a get method with the provided link and checking whether is successful or not. After create the general HTML/5 layout and start adding features regarding the task.

In addition, stylish features need to be crafted manually such as svg, css.

__

Requirements 

For the requirements of the task such as “A title (no more than 200 characters in length)” or format of the date, i created filter with vuejs.

Furthermore, in the index page, i handled the behaviour of the DOM with the v-directories (v-if, v-else).

For example, the pullQuote or paragraphPosition.

 

CSS3 Stylish

For my development regarding the task, i created custom css3 rules for the need of the layout and the elements. Moreover, i hand crafted svg rectangle shape dynamically responsive with resolutions. 

__

Finally, the implementation with all the required features regarding the code.test.rtf and the layouts is done then a test on the stylish and the functionality is performed. 

Testing

The webpage has been tested for iPad, iPhone and cross browser compatibility with the same resolutions. 