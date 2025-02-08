
<img width="628" alt="Screenshot 2025-02-09 at 01 33 36" src="https://github.com/user-attachments/assets/98614497-6519-4a6e-adea-d18e95c81052" />

## Birthday Buddy - React Fundamental Project 1

Birthday Buddy is a simple React application that displays a list of people with their birthdays. Users can view the list of people and clear the list with a button click.

** Online Live:** https://birthday-buddy-arnob.netlify.app/

## Getting Started

### Installation

1. Clone the repository.
2. Navigate to the project directory.
3. Install the dependencies:

```sh
npm install
```

### Running the Project

To start the development server, run:

```sh
npm run dev
```

## Components

### App.jsx

The main component that sets up the state and renders the list of people. It also includes a button to clear the list.

### List.jsx

A component that receives the list of people as props and maps over them to render each person using the `Person` component.

### Person.jsx

A component that receives individual person data as props and renders the person's image, name, and age.

## Styling

The project uses a global CSS file (`src/index.css`) to style the components. The CSS includes variables for colors, fonts, and other design elements.

## Data

The data is imported from data.js, which contains an array of objects representing people with their `id`, `name`, `age`, and `image` URL.

## Functionality

- **Display List**: The list of people is displayed with their images, names, and ages.
- **Clear List**: A button allows users to clear the list of people.

## Project Detail Steps

### Import Data

In App.jsx, import the data (from data.js) to be rendered as an array of objects. Each object should represent a person and contain properties such as name, age, and image URL.

### Setup State Variable

Then, set up the data as a state variable using the useState hook. This will allow the data to be modified and have those changes automatically reflected in the rendered output.

### Iterate and Render

Display the number of items in the list by using the length property of the state variable. This information can be displayed using plain text or added to a message or heading element.

To render the list of people, iterate over the data array using the map method. For each item in the array, render an image element (hint : use inline styles to make width smaller).Additionally, render the person's name and age as plain text.

Create a List component to hold the rendered items. This component can be a simple div element containing the list of Person components.

Create a Person component to render the information for each person. This component should receive the person data as props and render the image, name, and age information.

### Clear List

In App.jsx, add a button to clear the list, and set up the functionality by defining a function that resets the state variable to an empty array.

Overall, the flow of the application should look something like this:

- Import the data you want to render in App.jsx.
- Set up the data as a state variable using useState.
- Use the map method to iterate over the data array and render a Person component for each person.
- Each Person component should render an image with a style prop to control the width, the person's name, and the person's age.
- Create a List component that holds the rendered items.
- Create a button with functionality to clear the list.
- Display the number of items in the list using the length property of the state variable. This can be rendered using plain text or added to a message or heading element.
