# Random-Jokes-Generator
![Screenshot 2024-09-03 132604](https://github.com/user-attachments/assets/303c2edd-9292-4f8f-ba31-e07608ace897)

## This React component, Random, is designed to fetch and display a random joke from an external API. Here’s a summary of the code:

1. State Management:

* The component uses the `useState` hook to manage the `randomJokes` state, which stores the fetched joke.
2. Fetching Data:

* The `showJokes` function is an asynchronous function that fetches data from the "Official Joke API" using `fetch`. If the request is successful, it updates the `randomJokes` state with the fetched joke. If there is an error during fetching, it logs the error to the console.
3. Effect Hook:

* The `useEffect` hook calls the `showJokes` function once when the component mounts, ensuring that a joke is fetched as soon as the component loads.

4. Conditional Rendering:
* the component displays a "Loading..." message before the data is fetched. Once the joke is fetched and stored in the `randomJokes` state, it conditionally renders the joke's `setup` and `punchline`.
5. Joke Display:

* The joke is displayed within a styled div. The user can fetch a new joke by clicking the "Show Jokes" button, which triggers the `showJokes` function again.
6. Styling:

The component includes various Tailwind CSS classes for styling the text, buttons, and layout.
