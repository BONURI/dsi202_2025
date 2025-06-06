# Rent Near Tu

## Abstract

Housing is a fundamental factor that significantly affects quality of life, especially for populations with income constraints, such as students, laborers, or middle- to low-income families. These groups often face difficulties accessing affordable rental housing that meets their needs, particularly in areas near Thammasat University, where there is high demand for accommodation. However, current systems for finding rental housing still lack centralized information and flexibility in selecting accommodations based on budget and real-life living factors.

In response to this problem, the developers have created a web application called Rent Near Tu as a solution to assist income constrained individuals in conveniently and efficiently finding rental rooms or dormitories near Thammasat University. This application is developed using Django, a framework well suited for systems that require organized data management. It is designed to serve both tenants and landlords. Tenants can search for accommodations based on their budget, desired basic amenities, and make reservations, while landlords can directly list their properties, ensuring that the system contains up-to-date and diverse information. The system is designed to be user friendly to maximize the efficiency of accommodation searches.

This project not only focuses on using technology to facilitate the search for housing but also has a social goal reducing inequality in access to housing for those with low incomes or limited resources. It aims to alleviate financial burdens, increase residential stability, and create opportunities for education and employment in the long term. Furthermore, the system has the potential to be scaled and applied in other areas with similar population characteristics and issues in the future.

---

## User Stories and User Steps

### Tenant user story:
Tenants can find suitable accommodations at affordable prices and view room amenities in detail to plan for additional purchases appropriately.

### User Steps:
1. Start by searching for a room using keywords such as dormitory name, price range, or preferred location.
2. Select a room of interest from the displayed list.
3. Carefully review room details such as rental price, included furniture, contract duration, and landlord contact information.
4. Click the “Book This Room” button to proceed with the reservation.
5. Choose your desired move in date.
6. Confirm your booking.
7. Make a payment via QR code to officially.




### Landlords user story 1:
Tenants can switch their role to landlords in order to post rental listings by themselves.

### User Steps:
1. Go to your personal profile page.
2. Select the “Apply to be Landlord” menu option.
3. Fill in the additional information as required by the system.
4. Once the application is approved, your role will be changed to landlord.
5. Add room details for rent, such as dormitory name, price, amenities, and number of rooms.
6. Check and manage the status of your listed rooms through your profile page.

### Landlords user story 2:
Landlords can provide detailed information about the room, such as room size, furniture, and rental price, so that tenants receive complete and accurate information.
### User Steps:
1. Log in as a landlord.
2. Add a new room with details 
3. Check the status and manage rooms through the profile page.

---
# UX/UI design

## User Flow Diagram
Mobile-optimized flows for tenant and landlord interactions.  


## Sitemap
Logical navigation structure for efficient user journeys.  

## Wireframe
Polished UI designs showcasing the app’s aesthetic and functionality.  


## Prototype
Prototype tested to evaluate user experience, with a strong focus on optimal usability.

## Color Theme
The app uses a black, white and blue color scheme to create a clean, minimalist look that reflects professionalism.

## Font
Inter, a modern font that emphasizes clarity and readability. It is well-suited for display across all devices, including smartphones and computers.



---

## Installation and Usage

## 1. **Clone the Project from GitHub**

1. 
   ```bash
   git clone https://github.com/BONURI/dsi202_2025.git
   cd myproject
   ```

## 2. **Standard Installation**
1. Set up the Database
   ```bash
   python manage.py migrate
   ```

2. Create a Superuser Account
   ```bash
   python manage.py createsuperuser
   
3. Run the Development Server
   ```bash
   python manage.py runserver
   
* Access the app: [http://localhost:8000/](http://localhost:8000/)
* Admin panel: [http://localhost:8000/admin/](http://localhost:8000/admin/)

## 3. **Set Up Google OAuth2 Login**

### Steps to Set Up:

1. Visit the [Google Cloud Console](https://console.cloud.google.com/)

2. Create a new project, or select an existing one.

3. Navigate to:  
   `APIs & Services`>`Credentials`>️ `Create Credentials`>️ `OAuth 2.0 Client IDs`

4. Select Web application, and add `http://localhost:8000` to Authorized JavaScript origins and `http://localhost:8000/accounts/google/login/callback/` to Authorized redirect URIs.
5. copy the generated `Client ID` and `Client Secret`.
6. Create a `.env` file in your project root and add the following:
   ```env
     SOCIAL_AUTH_GOOGLE_OAUTH2_KEY=YOUR_CLIENT_ID
     SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET=YOUR_CLIENT_SECRET
     ```
7. **Important**: Make sure to add `.env` to your `.gitignore` file to **keep your credentials safe** from being committed to version control.


---
## Youtube
DSI202 FINAL PROJECT:RENT NEAR TU
https://youtu.be/gozVwh4X_P4?si=zwVlh33oh5PXRo1o

---

## Conclution
The “Rent Near Tu” project is a web application developed to help reduce housing inequality for low income groups such as students and laborers. By leveraging technology, it facilitates a comprehensive and convenient platform for finding and offering rental accommodations near Thammasat University. The system supports both tenants and landlords, enhancing residential stability, reducing financial burdens, and promoting long term opportunities for education and employment. Furthermore, the system can be expanded to other areas facing similar housing challenges in the future.

