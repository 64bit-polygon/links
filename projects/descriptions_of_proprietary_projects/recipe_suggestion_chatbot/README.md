# [← Back to repo list](https://github.com/64bit-polygon/links)

# Recipe suggestion chatbot

In 2023, I led a team in a company-wide hack-a-thon at WeightWatchers that won first place. The project was built using `React`. We produced a chatbot using `ChatGPT` that suggests existing recipes in the WW database and acted as a smart/suggested search. In addition to leading the team, I was the sole front end engineer and I outlined how the data would flow. 

Here is how it worked:

The user would ask a question such as "What are some vegan summer dishes" or "Give me some orange colored main dishes" or "Give me an authentic Chinese side dish using tomatoes", etc. Using the user input, we'd create a prompt to get sent to the `ChatGPT` endpoint. We engineered the prompt to ensure we'd always get back a list of recipes from the input (unless the user asked something off-topic, then we'd inform the user). Taking the list of recipes, we'd query the WW search endpoint for recipes and display the topic result for each recipe.

Additionally, along with providing the list of recipes, we instructed `ChatGPT` to return a recipe as well. The recipe would include an `array` of `objects` for the ingredients. Each object would hold an ingredient name, and quantity, and a unit type (cups, grams, etc.). Using those ingredients, we'd search the WW food database for each of those ingredients, collect all of their results, and display a recipe the user could save onto their account. This is important bc WeightWatchers uses a points system to track foods, as such each ingredient needs an accurate point amount to make the recipe.

Lastly, if there was not an image attached to the results from the WW database, one would be created via `DALL-E`, the text to image service. All fully generated recipes were paired with `DALL-E` images.

<a href="https://firebasestorage.googleapis.com/v0/b/react-portfolio-944de.appspot.com/o/recipe-suggestion-chatbot.mp4?alt=media&token=944a35c4-bca7-42b7-adff-83d6f947cd22" target="_blank">Here is a screen recording</a> of the project.