# 🚀 React URL Shortener

A modern, fully client-side URL shortener built using **React** and **Material UI**, offering a seamless way to create, manage, and track short links — all within your browser. Designed with performance, usability, and privacy in mind, this application functions without any backend or server dependency.

Whether you're looking to generate compact URLs for sharing, monitor click analytics, or manage a personal collection of shortened links, this tool provides a streamlined and efficient experience with zero setup required.

---

## ✨ Why This Project Stands Out

- ✅ **No Backend Required** — Everything runs entirely in your browser using `localStorage`. No sign-ups, no servers, no databases.
- 🎯 **Smooth User Experience** — Intuitive design with real-time validation, responsive layout, and one-click interactions.
- 📊 **Powerful Features** — Includes click tracking, expiry management, analytics dashboard, and custom shortcode support.
- 🧠 **Performance Optimized** — Handles multiple URLs with ease using concurrent processing and smart storage techniques.
- 🔒 **Private by Design** — All data stays local to your device. Nothing is shared externally.

---

## 📸 Dashboard Preview

Explore key sections of the application in action. Click any image to view in full size.

<table> <tr> <td align="center"> <a href="https://github.com/user-attachments/assets/eaa24f4f-7452-4f12-92e0-d4ebd39c4ad2" target="_blank"> <img src="https://github.com/user-attachments/assets/eaa24f4f-7452-4f12-92e0-d4ebd39c4ad2" width="280" alt="Main Dashboard" /> </a><br/> <sub><b>Main Dashboard</b></sub> </td> <td align="center"> <a href="https://github.com/user-attachments/assets/fad123ec-d9e9-4741-b613-6cdecc5dc715" target="_blank"> <img src="https://github.com/user-attachments/assets/fad123ec-d9e9-4741-b613-6cdecc5dc715" width="280" alt="URL Shortener" /> </a><br/> <sub><b>URL Shortener</b></sub> </td> <td align="center"> <a href="https://github.com/user-attachments/assets/6089f65e-6c8b-4c80-aefb-d494c8074369" target="_blank"> <img src="https://github.com/user-attachments/assets/6089f65e-6c8b-4c80-aefb-d494c8074369" width="280" alt="Recent URLs" /> </a><br/> <sub><b>Recent URLs</b></sub> </td> </tr> <tr> <td align="center"> <a href="https://github.com/user-attachments/assets/e31e822d-aed3-4536-b9fa-30f15214cbbf" target="_blank"> <img src="https://github.com/user-attachments/assets/e31e822d-aed3-4536-b9fa-30f15214cbbf" width="280" alt="Detailed Analytics" /> </a><br/> <sub><b>Detailed Analytics</b></sub> </td> <td align="center"> <a href="https://github.com/user-attachments/assets/0859ca73-e1eb-4158-942e-a7e1725e5f24" target="_blank"> <img src="https://github.com/user-attachments/assets/0859ca73-e1eb-4158-942e-a7e1725e5f24" width="280" alt="URL Statistics" /> </a><br/> <sub><b>URL Statistics</b></sub> </td> <td></td> </tr> </table>

---

## 🤔 How It Works

This project is a **client-side only** application. Instead of relying on a backend server and database, it leverages your browser's **`localStorage`** for all data storage.

1.  **Shortening:** When you shorten a URL, the app generates a unique shortcode and stores the mapping (`shortcode` -> `original URL`) in `localStorage`.
2.  **Redirection:** The shortened link uses a URL hash fragment (e.g., `https://your-app.com/#/yourshortcode`). When visited, the React application reads the shortcode from the URL, looks up the original URL in `localStorage`, records a click, and then redirects the user.

This approach ensures total privacy and zero server costs.

---

## 🌟 Key Features

* **Serverless by Design:** All logic and storage are handled in the browser.
* **Custom Shortcodes:** Personalize your links with memorable aliases.
* **Expiry Dates:** Set links to expire automatically after a specified duration.
* **Click Analytics:** Track link performance with a built-in click counter.
* **Advanced Management:** A detailed dashboard to search, filter, and manage links.
* **Batch Processing:** Shorten up to 5 URLs at once.
* **Data Export:** Backup all your link data to a single JSON file.
* **PWA Ready:** Installable as a standalone application for easy access.

---

## 🛠️ Built With

This project is built with modern web technologies.

<p align="left">
  <a href="https://reactjs.org/" target="_blank">
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React"/>
  </a>
  <a href="https://mui.com/" target="_blank">
    <img src="https://img.shields.io/badge/Material--UI-007FFF?style=for-the-badge&logo=mui&logoColor=white" alt="Material UI"/>
  </a>
  <a href="https://reactrouter.com/" target="_blank">
    <img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" alt="React Router"/>
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  </a>
</p>

---

## 🏗️ Project Structure

The source code is organized to separate concerns, making it clean and maintainable.

```
src/
├── components/         # Reusable React components (Forms, Tables, Cards)
│   ├── ShortenerForm.jsx
│   ├── StatisticsTable.jsx
│   └── RedirectHandler.jsx
├── pages/              # Main pages of the application
│   ├── ShortenerPage.jsx
│   └── StatisticsPage.jsx
├── utils/              # Helper functions and utilities
│   ├── storage.js      # localStorage management
│   └── urlUtils.js     # URL validation and processing
├── App.js              # Main component with routing logic
└── index.js            # Application entry point
```

---

## 🚀 Getting Started

### Prerequisites

* Node.js (v14 or higher)
* NPM or Yarn

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/react-url-shortener.git](https://github.com/yourusername/react-url-shortener.git)
    cd react-url-shortener
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Run the development server:**
    ```bash
    npm start
    ```
    The app will be available at `http://localhost:3000`.

### Build for Production

To create a static, production-ready build:
```bash
npm run build
```
This command bundles the app into the `build/` directory.

---

## 🚢 Deployment

Deploy the contents of the `build/` folder to any static hosting service.

**Important**: Since this is a single-page application (SPA), you must configure your host to redirect all paths to `index.html`. This ensures that direct navigation to a short link (e.g., `your-site.com/#/shortcode`) works correctly.

* **Netlify:** Create a `_redirects` file in your `public/` folder with: `/* /index.html 200`
* **Vercel:** No configuration needed; it's handled automatically.

---

## 🤝 Contributing

Contributions are welcome! If you have a feature request or find a bug, please open an issue or submit a pull request.

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature-name`).
3.  Make your changes and commit them (`git commit -m 'Add some feature'`).
4.  Push to the branch (`git push origin feature/your-feature-name`).
5.  Open a Pull Request.

---

✍️ Author
<table> <tr> <td align="center"> <a href="https://github.com/22bq1a42d4"> <img src="https://avatars.githubusercontent.com/22bq1a42d4" width="100px;" alt="Seelam Abhinav GitHub"/><br /> <sub><b>Seelam Abhinav</b></sub> </a><br /> 💻 Full-Stack Developer & AI Enthusiast <br/> 🔗 <a href="https://github.com/22bq1a42d4">@22bq1a42d4</a> </td> </tr> </table>


---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
