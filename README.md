# GlobalStore – Full-Stack Internationalization Demo

GlobalStore is a simple, professional project that demonstrates how internationalization works across both the frontend and backend of an application.

## What the project demonstrates

- English, Tamil and Hindi language switching
- Frontend interface translation
- Localized product data returned by a Node.js API
- Locale-aware currency and date formatting with `Intl`
- Language preference saved in `localStorage`
- Responsive and accessible user interface
- `Accept-Language` and query-parameter language handling

## Technology used

- HTML
- CSS
- JavaScript
- Node.js
- Express

## How to run

1. Open the project folder in VS Code.
2. Open the VS Code terminal.
3. Install the dependency:

   ```bash
   npm install
   ```

4. Start the application:

   ```bash
   npm start
   ```

5. Open this address in your browser:

   ```text
   http://localhost:3000
   ```

6. Use the language menu to switch between English, Tamil and Hindi.

## What to show in a demo

1. Start on the English version.
2. Open the browser's Developer Tools and select the Network tab.
3. Change the language to Tamil.
4. Show that both the interface and product information change.
5. Open the `/api/products?lang=ta` request and show the localized JSON response.
6. Refresh the page and show that the selected language remains saved.

## Important files

- `server.js`: Backend API, language detection and translated product data
- `public/app.js`: UI translations, language switching, API calls, date and currency formatting
- `public/index.html`: Application structure
- `public/styles.css`: Responsive visual design

## API examples

```text
GET /api/products?lang=en
GET /api/products?lang=ta
GET /api/products?lang=hi
GET /api/status?lang=ta
```

This demo keeps translations directly in the source code so beginners can understand the complete flow. Larger production applications normally keep translations in separate locale files or use libraries such as i18next.
