### Description
Your task is to develop a one-page application with a list of tweets and display
the information related to tweets using VueJS and Vuex. To access the data use 
the `axios` library. It is not recommended to use any CSS frameworks (Bootstrap,
Materialize CSS), because our secondary task is to test your CSS skills.

### **What should be done?**
- Configure webpack (minimize plugin, vue-loader, scss-loader, babel, etc.)
- Configure the json-server, see the documentation on github 
[json-server](https://github.com/typicode/json-server). To run this json-server 
you can simply run `npm run db-server` command configured in `package.json`
- Use **SCSS**. Your **SCSS** styles should be in separate files.
- Responsive design, as a result your application should have a mobile version 
and desktop version.
- The main font is **_Montserrat_**. You can find this font on the Google Fonts service.
- Interface should be in English.
- It is necessary to note the execution time from the moment of familiarization
with the task until the end of the execution. This is important to evaluate your performance.
- Work in GitHub, make as many commits as possible, each commit should
clearly describe the completed subtask.

The layout could be found in the file `mockup.pdf`. The layout shows just the 
location of the elements, you integrate the design by yourself, at your discretion.

In the json file you will find data about tweets (`db/tweets.json`). 
At the top of the layout should be a search for tweets, the search is performed 
in accordance with the selected type: `by tweet text`, `by hashtag`, `by user name`
+ one parameter (preferably numeric), chosen by you. If we perform the search,
the found date should be _highlighted_ in text of tweets. It is also required to implement
filtering by language (each tweet has this parameter), a list of languages is 
displayed based on the languages available in tweets (there may be others 
besides en and fr). The “**count**” value should be updated after any filtering
of tweets. The tweets themselves should be displayed on the left side of the screen,
pagination should be applied to tweets, and after each filtering the pagination 
should also be **updated**. At the right bottom make a selection of the number 
of tweets displayed on the page (read about `json-server` **slice**). Clicking
on a specific tweet on the right should display information about the user who
made the tweet (5 data minimum). It is also necessary to display a photo of the 
user profile, if it doesnt exist, or the link is not available, then display 
the standard photo selected by you. In the lower right corner you need to display
the following information about tweets: _the number of retweets_, 
_the number of added to favorites_, and if the data exists, you should display:
 _hashtags_, _tagged users_, _links_ that are in tweet, information on _retweets_. 
Tweets can be **deleted**, selected tweets should be deleted by clicking on 
the “**Delete selected**” button. As for the _mobile_ version, it is implemented
at your discretion with a convenient UX and UI (preferably modal windows divided
 into blocks to display information on tweets).