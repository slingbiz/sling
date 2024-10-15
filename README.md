<div align="center">
  <h1>Sling: Open Source CMS for Developers</h1>
</div>

<div align="center">
  <img src="https://sling.biz/assets/images/sling_biz_sling_image.jpg"/>
</div>

<p align="center">
  <strong>
    <a href="https://studio.sling.biz">🚀 Live Demo</a>
  </strong>
</p>

Sling is an open-source drag-and-drop frontend CMS built on Next.js. Completely customizable with Pages, Templates & Widgets written in React. Sling offers an alternative to Builder.io, designed for developers who want full control over their components and frontend experience.

## ✨ Features :fire:

- **React & Node.js**: Built entirely with React on the frontend and Node.js on the backend.
- **Complete Control**: Manage React components and their props directly from Sling Studio.
- **Custom Widgets**: Create and modify custom widgets within your page templates.
- **Modular Architecture**: Sling consists of three main repositories:
  - **Sling API**: The backend API managing all data handling and communication.
  - **Sling FE**: The frontend, handling page rendering and routing.
  - **Sling Studio**: The admin interface where users can manage content and create widgets visually.

## 🛠️ Prerequisites

To properly set up Sling, you need:

- **MongoDB URI**: Make sure you have a MongoDB instance running and obtain its URI.
- **Node.js**: Ensure you have Node.js version 18 or greater installed.

## 🚀 Setting up Sling - Hosted Studio

To set up a Sling project locally using [Hosted Studio](https://studio.sling.biz/), follow these steps:

### Frontend App Setup

1. **Use the Installer**:
   - Create the Sling Frontend app by running the following command:
     ```sh
     yarn create sling-app my-project
     ```
   - Follow the prompts to configure your Sling app.

2. **Obtain Sling Studio Keys**:
   - Visit [Sling Studio](https://studio.sling.biz/) and sign up to create an account.
   - Complete the company setup.
   - Navigate to your account settings or profile section.
   - Locate the section for accessing or generating Sling Studio Keys.
   - Copy the keys provided and update them in the `.env` file for the frontend app.
   - **Voilà!** You can now access your app at [http://localhost:4087](http://localhost:4087).

3. **Play Around**:
   - Access [Sling Studio](https://studio.sling.biz/).
   - **Create custom widgets** and use them in your page templates.
   - **Modify content from Studio** and see the changes instantly in your frontend app.

## 🌐 Setting up Sling - Self-Hosted Studio

If you prefer to host Sling Studio on your local machine, Sling consists of three primary parts: **Sling Studio**, **Sling API**, and **Sling FE**.

### Step-by-Step Setup:

1. **Run the Installer**:
   - Use the installer to set up the Sling project by running:
     ```sh
     yarn create sling-app my-project
     ```
   - Follow the prompts to configure your Sling app, selecting the self-hosted option.

2. **Start the Services**:
   - After running the installer, services will be started in the background, but you can manually run them:
     - Frontend: `cd sling-fe && npm run dev`
     - Studio: `cd sling-studio && npm run dev`
     - API: `cd sling-api && npm run dev`

3. **Access the Application**:
   - Frontend: `http://localhost:4087`
   - Studio: `http://localhost:2021`
   - API: `http://localhost:10001`

## 📂 Project Structure

Sling is structured across three separate repositories, each serving a key function:

1. **[Sling API](https://github.com/yourusername/sling-api)**:
   - Handles backend logic, including database connections and API endpoints.
   - Built on Node.js and MongoDB for scalable backend services.

2. **[Sling Frontend (sling-fe)](https://github.com/yourusername/sling-fe)**:
   - The frontend where all the pages, routing, and widget rendering take place.
   - Built with Next.js, allowing developers to customize their pages and integrate widgets dynamically.

3. **[Sling Studio](https://github.com/yourusername/sling-studio)**:
   - Admin interface where users can create, edit, and manage content visually.
   - Allows for real-time page editing with drag-and-drop capabilities for widgets and templates.

By separating these concerns, Sling allows developers to work on specific parts independently while ensuring seamless integration between the frontend, backend, and admin interface.

## 📚 Documentation

- [Website](https://sling.biz)
- [Documentation](https://sling.biz/documentation/)
- [Demo](https://studio.sling.biz)

## 🙋 Getting Help

If you have any questions or something you'd like to discuss, feel free to join our [Slack](https://slingbiz.slack.com/archives/C06KE4ZMSQP) channel.

Alternatively, you can raise a [GitHub issue](https://github.com/slingbiz/sling-fe/issues), or reach out directly to the author via [Email](mailto:ankur@sling.biz) or [LinkedIn](https://www.linkedin.com/in/ankurpata/).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
