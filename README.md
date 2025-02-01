# WhatsApp-API-Integration
How to Send WhatsApp Messages With Laravel 11?

### Step 1: Clone Project
```bash
git clone https://github.com/ruhulamin63/WhatsApp-API-Integration.git
```

### Step 2: Copy .env
```bash
cp .env.example .env
```
### Step 3: Create DB
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your-db-name
DB_USERNAME=root
DB_PASSWORD=
```
### Step 4: Set up a Twilio Account
First you need to create and add phone number. then you can easily get account SID, Token and Number.

Create Account from here: `www.twilio.com`.

Next add Twilio Phone Number

Next you can get account SID, Token and Number and add on .env file as like bellow:
```bash
TWILIO_SID=your_twilio_account_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_WHATSAPP_NUMBER=your_twilio_whatsapp_number
```

### Step 5: Install twilio/sdk Package
In this step, we need to install twilio/sdk composer package to use twilio api. so let's run bellow command:
```bash
composer require twilio/sdk
```

```bash
composer update
```

```bash
php artisan migrate
```

### Public Access Route
```bash
http://127.0.0.1:8000/whatsapp
```

#### ===Enjoy coding ====

*** Copyright@reserved by Ruhul Amin ***