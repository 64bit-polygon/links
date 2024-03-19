# [← Back to repo list](https://github.com/64bit-polygon/links)

# Program Assessment

A few years ago, I was tasked with building a user-facing assessment at WeightWatchers. The result of the assessment would suggest one of three plans to the user. The assessment was built in `React`, with the global state being handled with `Redux`. Although the assessment was built using web tools it was piped into the `iOS` and `Android` versions of the app, so one of the requirements was that it have a native look and feel. To do so, I used `CSS` animations (compiled from `SCSS`).

First, a call would be made to fetch a `JSON` with the questions in the assessment from our assessments service. The content of the assessment was contingent on the profile of the user: some countries asked different questions; many countries were non-English speaking; some would be new users; some would be existing users. The user would be return a different `JSON` file depending based on their profile, and thus experience a different assessment.

The user would answer a series of questions about their eating habits and daily routines. Their responses were then passed to the BE and one of three weight loss plans would be suggested. The plans allowed for a certain number of "points" they could use per day and per week, with more caloric foods given higher points, less caloric one lower points. The plan would have a personalized list of foods with no points that they would be free to eat whenever.

After taking the assessment, users would go through a tutorial to explain the plan suggested to them. They'd be given the option to select the suggested plan; retake the assessment; or choose one of the two other plans. 

This was a very engaging project for me. It was the type of project I enjoy working on: I had to think deeply about the architecture, as a project like this needs clear, clean logic. The rendered `React` components had to be versatile yet simple. And lastly it had to look beautifully and run smoothly as it was to be experienced on web, `iOS`, and `Android`.

You can see a screen recording of my general work on the WeightWatchers web app <a href="https://natedelacruz.com/weightwatchers">here</a>.