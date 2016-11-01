# Project 3 - *Name of App Here*

**Name of your app** is an android app that allows a user to view his Twitter timeline and post a new tweet. The app utilizes [Twitter REST API](https://dev.twitter.com/rest/public).

Time spent: **27** hours spent in total

## User Stories

The following **required** functionality is completed:

* [ Implemented ]	User can **sign in to Twitter** using OAuth login
* [ Implemented]	User can **view tweets from their home timeline**
  * [ Implemented ] User is displayed the username, name, and body for each tweet
  * [ Implemented ] User is displayed the [relative timestamp](https://gist.github.com/nesquena/f786232f5ef72f6e10a7) for each tweet "8m", "7h"
  * [ Implemented ] User can view more tweets as they scroll with [infinite pagination](http://guides.codepath.com/android/Endless-Scrolling-with-AdapterViews-and-RecyclerView). Number of tweets is unlimited.
    However there are [Twitter Api Rate Limits](https://dev.twitter.com/rest/public/rate-limiting) in place.
* [Implemented ] User can **compose and post a new tweet**
  * [Implemented ] User can click a “Compose” icon in the Action Bar on the top right
  * [ Implemented] User can then enter a new tweet and post this to twitter
  * [ Implemented] User is taken back to home timeline with **new tweet visible** in timeline

The following **optional** features are implemented:

* [Implemented ] User can **see a counter with total number of characters left for tweet** on compose tweet page
* [ Implemented] User can **click a link within a tweet body** on tweet details view. The click will launch the web browser with relevant page opened.
* [ Implemented] User can **pull down to refresh tweets timeline**
* [Implemented ] User can **open the twitter app offline and see last loaded tweets**. Persisted in SQLite tweets are refreshed on every application launch. While "live data" is displayed when app can get it from Twitter API, it is also saved for use in offline mode.
* [Implemented ] User can tap a tweet to **open a detailed tweet view**
* [ Implemented] User can **select "reply" from detail view to respond to a tweet**
* [ ] Improve the user interface and theme the app to feel "twitter branded"

The following **bonus** features are implemented:

* [ ] User can see embedded image media within the tweet detail view
* [ ] User can watch embedded video within the tweet
* [Implemented ] Compose tweet functionality is build using modal overlay
* [Implemented ] Use Parcelable instead of Serializable using the popular [Parceler library](http://guides.codepath.com/android/Using-Parceler).
* [ Implemented] [Leverage RecyclerView](http://guides.codepath.com/android/Using-the-RecyclerView) as a replacement for the ListView and ArrayAdapter for all lists of tweets.
* [ ] Move the "Compose" action to a [FloatingActionButton](https://github.com/codepath/android_guides/wiki/Floating-Action-Buttons) instead of on the AppBar.
* [ ] On the Twitter timeline, leverage the [CoordinatorLayout](http://guides.codepath.com/android/Handling-Scrolls-with-CoordinatorLayout#responding-to-scroll-events) to apply scrolling behavior that [hides / shows the toolbar](http://guides.codepath.com/android/Using-the-App-ToolBar#reacting-to-scroll).
* [ ] Replace all icon drawables and other static image assets with [vector drawables](http://guides.codepath.com/android/Drawables#vector-drawables) where appropriate.
* [ ] Leverages the [data binding support module](http://guides.codepath.com/android/Applying-Data-Binding-for-Views) to bind data into layout templates.
* [ ] Replace Picasso with [Glide](http://inthecheesefactory.com/blog/get-to-know-glide-recommended-by-google/en) for more efficient image rendering.
* [ ] Enable your app to [receive implicit intents](http://guides.codepath.com/android/Using-Intents-to-Create-Flows#receiving-implicit-intents) from other apps.  When a link is shared from a web browser, it should pre-fill the text and title of the web page when composing a tweet.
* [ ] When a user leaves the compose view without publishing and there is existing text, prompt to save or delete the draft.  The draft can be resumed from the compose view.

The following **additional** features are implemented:

* I've used greenDao as ORM

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='http://i.imgur.com/l3IuiEy.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while building the app.

## Open-source libraries used

- [Android Async HTTP](https://github.com/loopj/android-async-http) - Simple asynchronous HTTP requests with JSON parsing
- [Picasso](http://square.github.io/picasso/) - Image loading and caching library for Android
- GreenDao ORM

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.