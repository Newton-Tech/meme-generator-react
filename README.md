# Meme Generator

This is a simple meme generator built with React. It allows users to enter top and bottom text for a meme and generates a random meme image from the Imgflip API.

## How to Use

1. Clone the repository or download the source code.
2. Install the required dependencies by running `npm install` in the project directory.
3. Start the development server by running `npm start`.
4. Open your web browser and navigate to `http://localhost:3000`.
5. Enter the desired top and bottom text in the input fields.
6. Click the "Get a new meme image" button to generate a new meme with the entered text.
7. The meme image and the entered text will be displayed below the input fields.

## Dependencies

This project has the following dependencies:

- React: A JavaScript library for building user interfaces.
- react-dom: Provides DOM-specific methods that can be used with React.
- react-scripts: A set of scripts and configuration used by Create React App.

## Project Structure

- **index.js**: The entry point of the application. Renders the `Meme` component.
- **Meme.js**: The main component of the application. Handles state and renders the form and meme display.
- **styles.css**: Contains the CSS styles for the application.

## API Usage

The application uses the Imgflip API to fetch a list of available memes. The `useEffect` hook is used to fetch the memes from the API when the component mounts. The fetched memes are stored in the `allMemes` state variable.

To generate a new meme, the `getMemeImage` function is called when the "Get a new meme image" button is clicked. It selects a random meme from the `allMemes` array and updates the `randomImage` state with the selected meme's URL.

## Development

To modify the code and customize the meme generator, you can make changes to the `Meme.js` file. You can add additional features, improve the UI, or modify the API integration as needed.

Feel free to explore and experiment with the code to create your own unique meme generator!

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more information.