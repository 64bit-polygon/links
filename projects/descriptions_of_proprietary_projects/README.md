# Project descriptions of proprietary projects

Since 2018 I've been a software engineer at WeightWatchers. Unfortunately the work I've done there has been closed source and so I can't can't share code samples from them.

In lieu of the code, here are summaries of 3 major projects I've been the sole or lead engineer on while at WW. By clicking into them you'll get a more detailed description of each project.

They are listed from most to least recent.

# [Recipe suggestion chatbot 🤖💬🥗](https://github.com/64bit-polygon/chat_bot)

In 2023, I led a team in a company-wide hack-a-thon at WeightWatchers that won first place. Utilizing the WeightWatchers DB, it suggested WW recipes based on user input and created full recipes on the fly the user could save. It also populated any missing images in search results with DALL-E. <a href="https://nate-de-la-cruz.dev/chatbot.mp4" target="_blank">Here's recording</a> of it.

`JS`, `React`, `Node.js`, `SCSS`, `Front end`

# [Applanga service](https://github.com/64bit-polygon/Applanga-Service)

This is a translations BE microservice. The 3rd party translations platform we use needs the data to be normalized and the fetching requires a lot of boilerplate. As teams across multiple platforms need the translations, this service reduces boilerplate, does the normalizing before it's sent, and keeps the data fresh.

`API`, `Back end`, `JS`, `Node.js`

# [Program assessment](https://github.com/64bit-polygon/program_assessment)

A few years ago, I was tasked with building an assessment while at WeightWatchers. The assessment would suggest one of three personalized plans to the user and provide onboarding. On top of running on the browser this project was piped into `iOS` and `Android` apps via web view so it had to have a native look and feel. The assessment was built in react, with their responses being stored in redux.

`React`, `Redux`, `Front end`, `JS`, `SCSS`
