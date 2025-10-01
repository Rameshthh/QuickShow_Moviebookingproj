## QuickShow 🌟

QuickShow is a full-stack movie ticket booking application built using Next.js (or MERN) and associated technologies. It enables users to browse movies, book tickets, and manage bookings, while providing an admin dashboard to manage the movie listings and bookings.

 Features

## User Side
- User signup / login (email, social, phone) using Clerk.
- Browse a list of currently showing movies, see details, and view screening times.
- Select seats & book tickets.
- Payment integration with retry logic: if payment fails, seats are held temporarily (~10 min) and released if not completed.
- Booking confirmation & reminder emails (via background jobs).
- View booking history, cancel, etc.

## Admin / Dashboard
- Add new movies (title, description, poster, genres, durations, showtimes).  
- Manage screening schedules.  
- View bookings, cancelations.  
- Send notifications / announcements to users when new movies are added.

 ## Backend / Infrastructure
- Background processing using **Inngest** for tasks like sending emails, scheduling reminders, handling booking expirations.
- Authentication & user management via **Clerk**.  
- Relational / document database for storing users, movies, bookings.  
- API endpoints for booking, payments, admin actions.    
- Real-time or polling (if needed) to reflect seat availability.

  ## THE SITE IS LIVE AT
  http://localhost:5173/
  https://quickshowmovie.netlify.app/
  https://quickshow.vercel.app/
