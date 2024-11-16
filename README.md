# BalanceBeam

**Finance Tracker** is an Android app designed to help you track your monthly financial transactions directly from your SMS messages. The app reads your SMS messages related to bank transactions, extracts relevant information such as the amount, type of transaction (spent, deposited, credited), and updates your balance. It also shows a detailed list of transactions for the current month.

## Features

- **SMS-Based Transaction Parsing**: Fetches SMS data from your inbox to identify financial transactions such as spending, deposits, and credits.
- **Transaction List**: Displays all transactions for the current month in a user-friendly list.
- **Total Expenditure Tracking**: Tracks the total amount spent based on the parsed SMS messages.
- **Current Balance**: Displays your current balance as extracted from relevant SMS messages.
- **Permissions Handling**: Asks for SMS permission to read your inbox and fetch transaction details.

## Screenshots

- Main screen displaying total expenditure and current balance.
- List of transactions with details such as date, type, and amount.

## Permissions

The app requires the following permissions to function properly:

- **Read SMS**: To access SMS messages from the device's inbox and parse transaction details.
  - Permission request is handled at runtime.

## Getting Started

To get started, download the app and follow the steps below:

1. **Grant SMS Permission**: The app will ask for permission to read SMS messages. You need to grant this permission for the app to fetch your financial transactions.
2. **View Transactions**: Once permission is granted, the app will automatically fetch the current month's transactions from your inbox.
3. **Monitor Spending**: The app will display your total spending and current balance in real-time, updating as new transactions come in.

## How it Works

- **SMS Data Parsing**: The app uses regular expressions to detect specific patterns in the SMS body, identifying spending, deposit, and credited transaction types.
- **Data Extraction**: It extracts the amount and transaction details, including the date and balance (if available) from the SMS content.
- **Transaction List**: The transactions for the current month are displayed in a list format using a `RecyclerView`.
- **Total Spent**: The app calculates the total amount spent based on the transaction data.

## Dependencies

- **Kotlin**: The app is built using Kotlin for better efficiency and readability.
- **Coroutine**: Used for background tasks, such as fetching and processing SMS data.
- **RecyclerView**: Used to display a list of transactions.

## How to Build

1. Clone this repository to your local machine.
2. Open the project in **Android Studio**.
3. Build and run the app on a physical Android device (SMS access is required).
4. Grant the necessary permissions when prompted.
   
## Future Improvements

- **Notifications**: Add notifications for low balance or overspending.
- **Data Storage**: Implement persistent storage to track spending over multiple months.
- **User Interface**: Enhance the UI for better user experience.

## Contributing

If you would like to contribute to this project, feel free to fork the repository and submit pull requests. All contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

You can now copy this README and use it for your project!
