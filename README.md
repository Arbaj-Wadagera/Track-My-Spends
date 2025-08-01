# Track-My-Spends Check_out_here    https://track-my-expenses-13z.web.app/ 
Track My Expenses: A modern, full-featured web application designed to help users manage their personal finances with ease. Built with vanilla JavaScript and powered by Google Firebase, this single-page application provides a seamless and responsive user experience for tracking expenses, setting budgets, and gaining financial insights. The integration of the Gemini API offers users personalized financial advice based on their spending habits.

Key Features Secure User Authentication: Full authentication system including user sign-up, login, logout, and password reset functionality, all handled securely by Firebase Authentication.

Comprehensive Expense Tracking: Users can add, delete, and view expenses. The interface allows for easy filtering of expenses by month and year, ensuring historical data is always accessible.

Advanced Budgeting: Set both an overall monthly budget and specific budgets for different categories (e.g., Groceries, Fuel, Rent). The dashboard provides a clear visual overview of spending against these budgets with progress bars.

AI-Powered Financial Coach: Leverages the Google Gemini API to provide users with personalized financial advice. Based on their monthly spending, the AI coach offers actionable tips to help them save money and improve their financial habits.

Persistent Data Storage: All user data, including profiles, expenses, and budgets, is securely stored in Cloud Firestore, ensuring data is never lost between sessions.

Professional Reporting: Generate and print clean, professional expense reports for any month. The report includes an overall summary, a detailed breakdown of category spending, and a list of all transactions.

Responsive Design & Theming: The application is fully responsive and works beautifully on desktop, tablet, and mobile devices. It also includes a user-toggleable Dark/Light theme for comfortable viewing in any lighting condition.

Technology Stack Frontend: HTML5, CSS3, Vanilla JavaScript (ES6 Modules)

Styling: Bootstrap 5

Backend & Database: Google Firebase

Firebase Authentication: For user management.

Cloud Firestore: As the NoSQL database for all application data.

AI Integration: Google Gemini API

Setup and Configuration To run this project locally, you will need to configure your own Firebase project and obtain a Gemini API key.

Clone the repository.

Create a new project in the Firebase Console.

Enable Authentication (with the Email/Password provider) and Cloud Firestore.

In the Firestore Rules, ensure that users are only allowed to read/write their own data.

In the Firestore Indexes, create a composite index for the expenses collection on userId (Ascending) and date (Descending).

Obtain your project's firebaseConfig object and paste it into the <script> tag in index.html.

Generate an API key from Google AI Studio and enable the Vertex AI API in your Google Cloud project.

Paste the Gemini API key into the apiKey constant within the getFinancialAdviceButton event listener in index.html.

Open the index.html file in your browser.
