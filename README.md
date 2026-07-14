✨ Anand Jyoti | Certified Life Coach

A premium, fully responsive, and dynamic coaching website built for Certified Life Coach Anand Labade. The project features a luxurious dark-glassmorphism UI, a complete client-facing frontend, and a fully functional, password-protected admin dashboard.

🚀 Live Features

🌐 Frontend (index.html)

Premium UI/UX: Dark mode aesthetic with golden gradients, glassmorphism cards, and smooth AOS scroll animations.

Dynamic Content: Sessions, Marquee ticker, and Gallery automatically update based on Admin Panel data.

Registration & Ticketing: Users can register for upcoming masterclasses via a dynamic modal.

Automated PDF Tickets: Automatically generates and downloads a beautifully designed PDF entry ticket using jsPDF.

Real Scannable QR Codes: Every ticket features a unique, sequentially generated QR Code (e.g., REG-SES123-001) using QRCode.js.

WhatsApp Contact Form: The contact form automatically formats user inquiries and redirects them to the official WhatsApp number.

🛡️ Admin Dashboard (admin.html)

Secure Access: Password-protected command center (Password: anandjyoti@11).

QR Ticket Scanner: Built-in webcam scanner using html5-qrcode. Scans digital/printed tickets, grants access, prevents duplicate entry (ticket reuse), and marks attendees as "Attended".

Session Management: Add, edit, or delete upcoming sessions. Changes instantly reflect on the frontend.

Registration Management: View all participants, filter by session/attendance status, and export data directly to .xlsx Excel files using SheetJS.

Gallery Management: Upload images directly to the homepage gallery. Built-in canvas compression prevents storage limits from being exceeded.

Local Database: All data is currently managed securely within the browser's localStorage.

🛠️ Tech Stack

Core: HTML5, Custom CSS3, Vanilla JavaScript (ES6)
Styling & UI: Bootstrap 5 (Grid/Layout), FontAwesome 6 (Icons), Google Fonts (Inter & Playfair Display)
Animations: AOS (Animate on Scroll)
Libraries (Loaded via CDN):

jsPDF (PDF Generation)

QRCode.js (QR Code Generation)

html5-qrcode (Admin Camera QR Scanner)

SheetJS / xlsx (Excel Export)

📁 File Structure

The entire application is architected to run perfectly from just two files and an images directory:

/
├── index.html       # The complete client-facing website
├── admin.html       # The password-protected admin dashboard
├── README.md        # Project documentation
└── /images
    ├── logo.png           # Transparent brand logo
    ├── herosection.jpg    # Premium hero background
    └── sir.png            # Transparent cutout of the coach


💻 Setup & Installation

Because this project utilizes advanced browser features (like Webcam access for the QR scanner and local storage APIs), it is highly recommended to run the project through a local web server rather than just double-clicking the HTML files.

Clone/Download the repository to your local machine.

Ensure you have the exact image files required in the /images folder.

Run a Local Server:

If using VS Code, install the Live Server extension, right-click index.html, and select "Open with Live Server".

Alternatively, use Python: python -m http.server 8000 (then visit http://localhost:8000).

Access Admin Panel: Navigate to admin.html and login using the master password: anandjyoti@11.

📱 Workflows to Test

Create a Session: Go to Admin -> Manage Sessions -> Add New Session. Fill out the details.

View on Frontend: Go back to index.html. Notice the Navbar, Marquee, and Upcoming Sessions section have updated automatically.

Register: Click "Register Now" on your new session. Fill out the form. A PDF ticket with a real QR code will download.

Scan Ticket: Open admin.html, go to "Scan Tickets". Point your camera at the QR code on your phone or printed PDF.

Verify: The system will mark the ticket as "Access Granted". If you scan it again, it will flash a warning that the ticket has already been used!

Export Data: Go to Admin -> Registrations -> Click "Download Excel" to see your attendees.

🔮 Future Roadmap (Upcoming Integrations)

The codebase has been specifically architected with placeholders to easily support the next phase of development:

[ ] Razorpay Integration: Real-time payment gateway on the registration modal.

[ ] WhatsApp Business API: Automated ticket delivery and confirmation messages via WhatsApp upon successful registration.

[ ] Backend Migration: Moving from localStorage to a persistent cloud database (Firebase/Supabase).

Designed & Developed for Anand Jyoti Showcase (July 2026).
