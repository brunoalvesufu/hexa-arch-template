
# 🚀 Hexagonal Architecture Template

Welcome to the **Hexagonal Architecture Template** repository! This is a well-structured and organized boilerplate for creating a backend project in JavaScript following the Hexagonal Architecture (Ports and Adapters). This template will help kickstart a project with a clean, scalable, and maintainable structure.

## 🗂 Project Structure

Here's a detailed overview of the project structure:

```
project-name/
│
├── public/
│   └── index.html
│   └── styles.css
│   └── script.js
│
├── src/
│   ├── application/
│   │   ├── usecases/
│   │   └── utils/
│   ├── domain/
│   │   ├── models/
│   │   ├── controllers/
│   │   └── logic/
│   ├── infra/
│   │   ├── db/
│   │   ├── entities/
│   │   ├── consumers/
│   │   ├── producers/
│   │   ├── clients/
│   │   └── servers/
│   └── presentation/
│       ├── index.html
│       ├── script.js
│       └── style.css
│
├── config/
├── tests/
├── scripts/
├── .env
├── .gitignore
├── package.json
└── README.md
```

## 📂 Folder Descriptions

### `src/`

This folder contains all the source code for the project.

### `src/application/`

Contains the application logic.

- **`usecases/`**: The core functionalities the application provides. Each use case typically has a class or module defining how that functionality should be executed.
- **`utils/`**: Auxiliary code with functions or structures used by the use cases to perform their tasks.

### `src/domain/`

Contains the core business logic of the application.

- **`models/`**: Classes or functions representing domain objects. These models define the data structure and basic rules they follow.
- **`controllers/`**: Functions that control the flow of data in the application. This directory can also be called "engine" or "motors".
- **`logic/`**: Functions implementing business logic that doesn't fit directly into models, like processing reviews to calculate an average.

### `src/infra/`

Handles infrastructure details and external integrations.

- **`db/`**: Database-related implementations.
- **`entities/`**: Mapping entities from the database or any other IO.
- **`consumers/`**: Message or event consumers.
- **`producers/`**: Message or event producers.
- **`clients/`**: Clients for external services.
- **`servers/`**: Server implementations (e.g., HTTP, WebSocket).

### `src/presentation/`

Contains the user interface.

- **`index.html`**, **`script.js`**, **`style.css`**: Basic front-end files.

### `config/`

Application configuration files. Define variables and settings that can change depending on the environment (development, test, production).

### `tests/`

Contains the application's tests. Organize unit, integration, and acceptance tests here to ensure each part of the code works as expected.

### `scripts/`

Useful scripts for automating tasks, like initial environment setup, build tasks, or deployment tasks.

### `.env`

Stores environment variables, like database connection settings, API keys, etc. These variables can differ for each environment (development, test, production).

### `.gitignore`

Specifies which files and folders should be ignored by Git. This typically includes auto-generated files, installed dependencies, and local settings that shouldn't be shared.

### `package.json`

Npm configuration file listing the project's dependencies, execution scripts, and other project settings. It's the central point for managing your Node.js project's dependencies and scripts.

### `README.md`

Provides an overview of the project, installation instructions, usage details, and other important information for developers working on the project or users wanting to understand it better.

## 🚀 Getting Started

To get started with this template, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/hexa-arch-template.git
    cd hexa-arch-template
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

3. **Run the server:**
    ```sh
    npm start
    ```

4. **Run tests:**
    ```sh
    npm test
    ```

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any changes you'd like to make.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Happy coding! 😊

