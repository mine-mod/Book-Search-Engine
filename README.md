# Book Search Engine

Welcome to the Book Search Engine! This application allows avid readers to search for new books to read, manage their saved books, and access personalized features. You can explore book titles, save your favorites, and manage your account seamlessly.

## Features

- **Search for Books**: Enter search terms to find books with detailed information including title, author, description, and images. You can also view a link to the book on the Google Books site.
- **User Authentication**: Sign up or log in to save books to your personal account.
- **Saved Books**: View and manage the books you have saved, including options to remove books from your list.
- **Logout**: End your session and return to the initial menu.

## User Stories

### As an avid reader
- **Search for New Books**: 
  - **Given** a book search engine
  - **When** I load the search engine
  - **Then** I see a menu with options to "Search for Books" and "Login/Signup," an input field to search for books, and a submit button.
  
  - **When** I click on "Search for Books"
  - **Then** I am presented with an input field to search for books and a submit button.
  
  - **When** I enter a search term and click submit
  - **Then** I see search results with book details, including title, author, description, image, and a link to Google Books.

- **Login/Signup**:
  - **When** I click on "Login/Signup"
  - **Then** a modal appears with options to log in or sign up.
  
  - **When** I toggle to "Signup"
  - **Then** I see inputs for a username, email, and password, plus a signup button.
  
  - **When** I toggle to "Login"
  - **Then** I see inputs for email and password and a login button.
  
  - **When** I enter a valid email and password to sign up
  - **Then** my account is created, and I am logged in.
  
  - **When** I enter my credentials to log in
  - **Then** I am logged in, and the modal closes.

- **Logged In Features**:
  - **When** logged in
  - **Then** the menu options change to "Search for Books," "See My Saved Books," and "Logout."
  
  - **When** I search for books
  - **Then** I see search results with a "Save" button for each book.
  
  - **When** I click "Save"
  - **Then** the book is added to my saved books list.
  
  - **When** I click "See My Saved Books"
  - **Then** I view a list of saved books with options to "Remove" each book.
  
  - **When** I click "Remove"
  - **Then** the book is deleted from my saved list.
  
  - **When** I click "Logout"
  - **Then** I am logged out and returned to the initial menu.

## Getting Started

To run the Book Search Engine locally, follow these steps:

1. **Clone the Repository**

    ```sh
    git clone <repository-url>
    cd Book-Search-Engine
    ```

2. **Install Dependencies**

    ```sh
    npm install
    ```

3. **Setup Environment Variables**

    Create a `.env` file in the root directory and add the following environment variables:

    ```env
    PORT=3000
    MONGODB_URI=<your-mongodb-uri>
    ```

4. **Start the Application**

    ```sh
    npm run start
    ```

5. **Open Your Browser**

    Navigate to `http://localhost:3000` to use the Book Search Engine.

## Technologies Used

- **Node.js**: JavaScript runtime for server-side logic.
- **Express**: Web framework for building APIs.
- **MongoDB**: NoSQL database for storing book data and user information.
- **Mongoose**: ODM library for MongoDB and Node.js.
- **Bootstrap**: Frontend framework for responsive design.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
