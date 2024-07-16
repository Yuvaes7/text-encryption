# Text Encryption and Decryption Application

This application allows you to encrypt and decrypt text using a simple web interface. It uses Node.js and Express for the backend and HTML, CSS, and JavaScript for the frontend.

## Features

- Encrypt text input
- Decrypt encrypted text
- User-friendly interface

## Installation

To get started with this project, follow the steps below:

### Prerequisites

Make sure you have the following installed:

- Node.js
- npm (Node Package Manager)
- Git

### Steps

1. **Clone the Repository**

    ```bash
    git clone https://github.com/Yuvaes7/text-encryption.git
    cd text-encryption
    ```

2. **Install Dependencies**

    ```bash
    npm install
    ```

3. **Set Up Environment Variables**

    Create a `.env` file in the root directory and add your secret key and initialization vector (IV) for encryption:

    ```env
    SECRET_KEY=your_secret_key_here
    IV=your_initialization_vector_here
    ```

4. **Install Git LFS (Large File Storage)**

    If you encounter issues with large files, make sure Git LFS is installed:

    ```bash
    sudo apt-get install git-lfs
    git lfs install
    git lfs track "*.css" "*.js"
    git add .gitattributes
    git add .
    git commit -m "Track large files with Git LFS"
    git push origin main
    ```

## Usage

1. **Start the Server**

    ```bash
    node index.js
    ```

    You should see the message: `Server is running on port 3000`.

2. **Open the Application**

    Open your web browser and go to `http://localhost:3000`.

3. **Encrypt Text**

    - Enter the text you want to encrypt in the "Text to Encrypt" field.
    - Click the "Encrypt" button.
    - The encrypted text will be displayed below.

4. **Decrypt Text**

    - Enter the encrypted text in the "Encrypted Text" field.
    - Click the "Decrypt" button.
    - The decrypted text will be displayed below.

## File Structure

```plaintext
text-encryption/
├── .env                  # Environment variables
├── .gitattributes        # Git LFS tracking
├── cryptoUtil.js         # Encryption and decryption functions
├── index.js              # Main server file
├── node_modules/         # Node.js modules
├── package.json          # Project dependencies
├── package-lock.json     # Lockfile for npm dependencies
├── public/               # Public assets (HTML, CSS, JS)
│   ├── index.html        # Frontend HTML
│   ├── styles.css        # Frontend CSS
│   └── scripts.js        # Frontend JavaScript
└── README.md             # Project documentation
```

## Contributing

Contributions are welcome! Please fork this repository and submit pull requests for any enhancements or bug fixes.

## License

This project is licensed under the MIT License.
