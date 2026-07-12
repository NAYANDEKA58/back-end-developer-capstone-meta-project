==================================================
LITTLE LEMON RESTAURANT PROJECT API - PEER REVIEW GUIDE HERE
==================================================

1. User Registration & Authentication (Using Djoser)
   - POST: http://127.0.0.1:8000/auth/users/ (Register users)
   - POST: http://127.0.0.1:8000/restaurant/api-token-auth/ (Obtain Token/Login)

2. Menu API Endpoints
   - GET / POST: http://127.0.0.1:8000/restaurant/menu/
   - GET / PUT / DELETE: http://127.0.0.1:8000/restaurant/menu/<id>

3. Booking API Endpoints (Token Authentication Header Required)
   - GET / POST: http://127.0.0.1:8000/restaurant/booking/tables/