# QuickStay

A modern hotel booking platform that connects travelers with unique accommodations worldwide. QuickStay provides an intuitive interface for guests to discover and book rooms, while offering hotel owners a comprehensive dashboard to manage their properties.

## 🏨 Features

### For Guests

- **Browse Hotels**: Explore a wide variety of accommodations
- **Room Details**: View detailed information about rooms with high-quality images
- **Easy Booking**: Seamless booking process with secure payment
- **My Bookings**: Track and manage your reservations
- **User Authentication**: Secure login and profile management

### For Hotel Owners

- **Property Management**: Register and manage hotel properties
- **Room Management**: Add, edit, and list rooms with detailed information
- **Dashboard Analytics**: Track bookings, revenue, and performance metrics
- **Booking Management**: View and manage guest reservations

## 🛠️ Tech Stack

### Frontend

- **React 19** - Modern React with latest features
- **Vite** - Fast build tool and development server
- **React Router DOM** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **Clerk** - Authentication and user management
- **Axios** - HTTP client for API requests
- **React Hot Toast** - Elegant notifications

### Backend

- **Node.js** - Runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database with Mongoose ODM
- **Clerk** - Authentication middleware
- **Stripe** - Payment processing
- **Cloudinary** - Image upload and management
- **Nodemailer** - Email notifications
- **JWT** - JSON Web Tokens for security
- **bcrypt** - Password hashing

## 📁 Project Structure

```
QuickStay/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React context for state management
│   │   └── assets/         # Images, icons, and static files
│   └── package.json
└── server/                 # Backend Node.js application
    ├── controllers/        # Business logic handlers
    ├── models/            # Database schemas
    ├── routes/            # API route definitions
    ├── middleware/        # Custom middleware functions
    ├── configs/           # Configuration files
    └── package.json
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- MongoDB database
- Clerk account for authentication
- Stripe account for payments
- Cloudinary account for image management

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/ASingha07/QuickStay.git
   cd QuickStay
   ```

2. **Setup Backend**

   ```bash
   cd server
   npm install
   ```

   Create a `.env` file in the server directory:

   ```env
   MONGODB_URI=your_mongodb_connection_string
   CLOUDINARY_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   CLERK_WEBHOOK_SECRET=your_clerk_webhook_secret
   STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
   STRIPE_SECRET_KEY=your_stripe_secret_key
   STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
   EMAIL_USER=your_email_user
   SMTP_USER=your_SMTP_user
   SMTP_PASS=your_SMTP_password
   ```

3. **Setup Frontend**

   ```bash
   cd ../client
   npm install
   ```

   Create a `.env` file in the client directory:

   ```env
   VITE_CURRENCY = $
   VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   VITE_BACKEND_URL=http://localhost:5000
   ```

4. **Run the Application**

   Start the backend server:

   ```bash
   cd server
   npm run server
   ```

   Start the frontend development server:

   ```bash
   cd client
   npm run dev
   ```

   The application will be available at `http://localhost:5173`

## 📱 Usage

### For Guests

1. **Sign Up/Login**: Create an account or login using Clerk authentication
2. **Browse Hotels**: Explore available accommodations on the home page
3. **Search & Filter**: Use filters to find hotels that match your preferences
4. **Book a Room**: Select dates, view details, and complete booking with Stripe
5. **Manage Bookings**: View and track your reservations in "My Bookings"

### For Hotel Owners

1. **Register Property**: Complete hotel registration to access owner dashboard
2. **Add Rooms**: Upload room details, images, and pricing
3. **Manage Listings**: Edit or remove existing room listings
4. **View Analytics**: Monitor bookings and revenue through the dashboard

## 🔧 API Endpoints

### Authentication

- `POST /api/users/webhook` - Clerk webhook for user management

### Hotels

- `GET /api/hotels` - Get all hotels
- `POST /api/hotels` - Create new hotel
- `PUT /api/hotels/:id` - Update hotel
- `DELETE /api/hotels/:id` - Delete hotel

### Rooms

- `GET /api/rooms` - Get all rooms
- `GET /api/rooms/:id` - Get room by ID
- `POST /api/rooms` - Create new room
- `PUT /api/rooms/:id` - Update room
- `DELETE /api/rooms/:id` - Delete room

### Bookings

- `GET /api/bookings` - Get user bookings
- `POST /api/bookings` - Create new booking
- `PUT /api/bookings/:id` - Update booking status

## 🎨 Design Features

- **Responsive Design**: Optimized for all device sizes
- **Modern UI**: Clean and intuitive user interface
- **Interactive Elements**: Smooth animations and transitions
- **Accessibility**: Built with accessibility best practices


## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**ASingha07** - [GitHub Profile](https://github.com/ASingha07)

## 🙏 Acknowledgments

- Thanks to all contributors who helped build this project
- Inspiration from modern booking platforms
- Open source community for the amazing tools and libraries

---

⭐ Star this repository if you find it helpful!
