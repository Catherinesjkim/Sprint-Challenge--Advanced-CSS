# Sprint Challenge: Advanced CSS - Space Walkers Web Page

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?

   Adaptive web design is different from responsive design in that there isn’t one layout that always changes. Instead, there are several distinct layouts for multiple screen sizes. And the layout used depends on the screen size used. For example, there could be a specific layout for mobile phones, tables, and desktop computers - each of which are made in advance. These three designs wait on standby until someone visits the site. The site detects the type of device used, and delivers the pre-set layout for that device. So instead of single ball going through several different-sized hoops, you’d have several different balls to use depending on the hopp size. 

  Responsive Web Design provides the optimal viewing experience of website, no matter what type of device the user is seeing it on. It’s an approach aimed at crafting sites to provide an optimal viewing experience--reading and navigation with a minimum of resizing, panning, and scrolling-across wide range of devices (from mobile phones to desktop computer monitors. This is done by using fluid grids. That’s a term for a design that works no matter what the screen size is. So no matter how much  you resize the screen, that same layout will automatically respond to that size, like a single ball growing or shrinking to fit through several different hoops.


2. Describe what it means to be mobile first vs desktop first.

  Mobile first is designed mainly for functionality. It’s a very focused approach starting with putting out a core function and layering the extras incrementally for higher resolutions. This strategy is often referred to as a content-first strategy because your website’s content must be carefully researched and structured to be categorized based on importance. This method can be more expensive due to the more extended preparation phase and the expertise needed to create the platform’s versatility. 

  Desktop first is a design for full sized screens, building for the highest specs to display and communicate as much as possible. In this design type it’s not the mobile but the desktop experience that needs to be detailed and dynamic. Going down to smaller resolutions means hiding and wrapping elements while trying to support as many original features as possible. In this case, the mobile experience is functional rather than refined. 


3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?

  Rem values are relative to the root html element, not to the parent element. That is, if font-size of the root element is 16px then 1 rem= 16px for all elements. If font-size is not explicitly defined in root element then 1 rem will be equal to the default font-size provided by the browser. A solution for this problem is percentage. Usually default font-size of the browser is 16px. Setting font-size: 100% will make 1 rem = =16px. But it will make calculations a little difficult. A better way is to set font-size: 63.5%. Because 62.5% of 16px is 10px. Which makes 1rem - 10px. 

4. How would you describe preprocessing to someone new to CSS?

  CSS Preprocessors are increasingly becoming a mainstay in the workflow of front end web developers. CSS is an incredibly complicated and nuanced language, and in an effort to make its usage easier, developers of turn to using preprocessors such as SAAS or LESS. CSS Preprocessors compile the code which is written using a special compiler, and then use that to create a css file, which can then be referenced by the main HTML document. 


5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

Favorite: When using any CSS Preprocessor, you will be able to program in normal CSS just as you would if the preprocessor were not in place, but you also have more options available to you. Nested syntax, ability to define variables, mixins, function, operational functions, joining multiple files, imports, escaping. 

Trouble: Parametric Mixins. 

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Follow these steps to set up your project:

### Git Set up

- [ ] Create a forked copy of this project.
- [ ] Add your project manager as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 

### Preprocessor Set up

* [ ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [ ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [ ] Add a viewport meta tag to the head of your index.html page

* [ ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [ ] Navigation Styles: Use the `navigation.less` file for styling.

* [ ] Main Content Styles: Use the `home-page.less` file for styling

* [ ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [ ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [ ]  Use at least 2 parameters to create your button

* [ ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [ ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription