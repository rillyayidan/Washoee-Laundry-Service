**Instructions:**

**Prerequisites**

To run this project, you need to have the following software installed on your computer:
- XAMPP (https://www.apachefriends.org/)
- Composer (https://getcomposer.org/)
- Laravel (https://laravel.com/)

**Installation Instructions**

1. **Setting Up XAMPP**
   1) **Download and Install XAMPP:**
   - Visit the XAMPP website and download the version suitable for your operating system.
   - Install XAMPP by following the installation guide.

   2) **Start Apache and MySQL:**
   - Open the XAMPP Control Panel.
   - Start the Apache and MySQL services.

2. **Setting Up the Project**
   1) **Download the Project Files:**
   - Download the Washoee project files from the provided Google Drive link.
   - Extract the files to the htdocs directory in your XAMPP installation (for example, C:\xampp\htdocs\Washoee).

   2) **Setting Up the Database:**
   - Open the XAMPP Control Panel and click the Admin button next to MySQL to open phpMyAdmin.
   - In phpMyAdmin, create a new database named `washoee_db`.
   - Import the database file located in the project directory: `C:\xampp\htdocs\Washoee\database\washoee_db.sql`.

   3) **Install Laravel and Composer Dependencies:**
   - Open the command prompt or terminal.
   - Navigate to the project directory (for example, use the command: `cd C:\xampp\htdocs\Washoee`).
   - Run the command `composer install` to install all the required dependencies.

   4) **Configure the Environment File:**
   - Rename the `.env.example` file to `.env`.
   - Open the `.env` file in a text editor and update the following lines to match your local environment:

   ```
   .env:
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=washoee_db
   DB_USERNAME=root
   DB_PASSWORD=
   ```

   5) **Run Database Migrations:**
   - In the command prompt or terminal, run the command `php artisan migrate`.

3. **Running the Project**

   1) **Run the Application:**
   - In the command prompt or terminal, run the command `php artisan serve`.
   - This will start the local development server. Note the server address (for example, `http://127.0.0.1:8000`).

   2) **Access the Project:**
   - Open a web browser and go to the server address (for example, `http://127.0.0.1:8000`).
   - You should see the Washoee home page.

4. **Additional Information**
1) **Public Assets:** Ensure the public directory contains all necessary assets such as CSS, JavaScript, and images.
2) **Blade Templates:** Blade template files are located in the `resources/views` directory.
3) **Controllers and Routes:** Controllers are located in the `app/Http/Controllers` directory.
4) **Routes** are defined in the `routes/web.php` file.
5) **CSS Files:** Custom CSS files are located in the `public/css` directory.
6) We use Laravel as the framework, so you need to install PHP, Laravel, Composer, etc.
