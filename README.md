# PowerBI & Jira API Integration with CI/CD

This project demonstrates how to integrate PowerBI with the Jira API, utilizing PHP and MySQL for backend operations. It also includes a CI/CD pipeline triggered by GitHub events.

## Features

- **Connect PowerBI to Jira:** Fetch and visualize Jira data in PowerBI reports.
- **Backend in PHP & MySQL:** Data processing and storage are handled with PHP scripts and a MySQL database.
- **CI/CD Integration:** Automated deployment and testing using GitHub Actions.

## Prerequisites

- PHP 7.x or higher
- MySQL 5.7 or higher
- PowerBI account
- Jira Cloud account with API access
- GitHub repository

## Setup Instructions

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/yourrepo.git
    ```

2. **Configure Environment Variables:**
   - Copy `.env.example` to `.env` and provide your database and API credentials.

3. **Install Dependencies:**
    - If you use Composer (for PHP packages):
        ```bash
        composer install
        ```

4. **Database Setup:**
    - Import the provided `schema.sql` to your MySQL instance.

5. **PowerBI Integration:**
    - Use the provided API endpoints as your data source in PowerBI.

6. **Jira API Setup:**
    - Generate an API token from your Jira account.
    - Update your `.env` file with the Jira API credentials.

7. **CI/CD Pipeline:**
    - The GitHub Actions workflow will automatically deploy and run tests on push or pull request events.

## Usage

- Run the PHP backend:
    ```bash
    php -S localhost:8000 -t public
    ```
- Access API endpoints as defined in the documentation.

## Contributing

Pull requests are welcome! For major changes, please open an issue first.

## License

[MIT](LICENSE)
