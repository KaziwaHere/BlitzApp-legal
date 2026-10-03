================================================================================
BLITZAPP - UNIFIED SPORTS & GAME CENTER BOOKING PLATFORM
================================================================================

1. OVERVIEW
--------------------------------------------------------------------------------
BlitzApp is a sports venue and recreation center booking platform designed for 
players, teams, and venue operators. It provides interactive venue discovery, 
real-time schedule management, and instant slot reservations with atomic 
conflict prevention.

The repository consists of:
- Flutter Frontend: Cross-platform mobile/web application (iOS, Android, Web).
- Laravel Backend: High-performance RESTful API backend with Laravel Sanctum 
  token-based authentication and MySQL database.


2. KEY FEATURES
--------------------------------------------------------------------------------
* Player & Team Booking:
  - Browse stadiums and game centers by city and neighborhood.
  - Interactive Google Maps venue pins and external navigation links.
  - Real-time time slot booking with atomic database locking to prevent 
    duplicate reservations.
  - Multi-language support: English and Central Kurdish (کوردی).
  - Favorites management, booking history, and in-app notifications.

* Venue Manager Portal:
  - List and update venue details, amenities, pricing in Iraqi Dinars (IQD), 
    and photos.
  - Capture accurate venue location coordinates via device GPS pin picker.
  - Manage daily operating schedules and block slots for private maintenance.
  - Receive booking alerts and review player no-show reports.

* Admin Console & Operations:
  - System-wide user and venue administration.
  - Dispute resolution tools and booking audit logs.
  - Platform service fee tracking (3% venue commission model).

* Security, Privacy & Compliance:
  - Bcrypt password hashing and token-based Sanctum authentication.
  - Rate-limited login endpoints.
  - Full self-service account deletion and data erasure compliance.
  - Text and in-app Legal Hub (Privacy Policy, Terms, Cancellation & Refund).


3. REPOSITORY STRUCTURE
--------------------------------------------------------------------------------
|
|-- privacy-policy.txt     # Plain text Privacy Policy
|-- terms-and-conditions.txt # Plain text Terms and Conditions
|-- cancellation-and-refund-policy.txt # Plain text Cancellation & Refund Policy
|-- about-legal.txt        # Plain text Legal & Compliance Overview
`-- README.txt             # Project documentation (this file)


4. QUICKSTART & RUNNING INSTRUCTIONS
--------------------------------------------------------------------------------
* Flutter Frontend Setup:
  1. Install dependencies:
     flutter pub get
  2. Generate localization files (if needed):
     flutter gen-l10n
  3. Launch the application:
     flutter run

* Laravel Backend Setup:
  1. Navigate to the backend directory:
     cd backend
  2. Install PHP dependencies:
     composer install
  3. Configure environment file:
     cp .env.example .env
     php artisan key:generate
  4. Run migrations and database seeders:
     php artisan migrate --seed
  5. Link storage directory:
     php artisan storage:link
  6. Start local development server:
     php artisan serve --port=8000
     (API available at http://127.0.0.1:8000/api/v1)


5. LEGAL & CONTACT
--------------------------------------------------------------------------------
Application: BlitzApp
Operator: Independent Project Operator (Personal Project)
Contact Email: blitz.platform.app@gmail.com
Jurisdiction: Kurdistan Region, Iraq
================================================================================
