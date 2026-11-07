# CSIT327-G1-PangueJr-Garry-FirstDjango

Full Name: Garry Pangue Jr.
Section: CSIT327 - G1

A simple Django application for a campus community. Users can create an account, log in, view the dashboard, and update their own profile.

## Run the application

1. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate   # Windows: .venv\Scripts\activate
   ```

2. Install dependencies:

   ```bash
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```

3. Apply database migrations:

   ```bash
   python manage.py migrate
   ```

4. Start the development server:

   ```bash
   python manage.py runserver
   ```

5. Open http://127.0.0.1:8000/ in your browser.

## Main pages

- Sign up: `/accounts/signup/`
- Log in: `/accounts/login/`
- Dashboard: `/`
- Edit your profile: `/accounts/profile/` (log in first)

## Notes

- The dashboard and profile page require login.
- Each user can edit only their own profile.
- Sign-up success messages are shown using Django's messages framework.
