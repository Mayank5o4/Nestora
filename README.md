# Nestora 🏠

A comprehensive travel and property management platform that combines property listings, video content, and intelligent trip planning. Nestora provides users with an all-in-one solution for discovering accommodations and planning their perfect getaway.

## 📋 Features

### Property Listings
- **List Properties** - Browse all available properties and accommodations
- **Create Listings** - Add new properties with detailed information
- **View Details** - See complete information about each property
- **Edit Listings** - Update property details and photos
- **Delete Listings** - Remove properties from the database

### Video Listings 🎥
- **Explore Destinations** - Watch engaging video content about travel destinations
- **Property Tours** - Video walkthroughs of available properties
- **Travel Inspiration** - Curated video content to inspire your next trip
- **Streaming Integration** - Seamless video playback experience

### AI Trip Planner 🤖
- **Smart Itineraries** - AI-generated travel plans based on your preferences
- **Personalized Recommendations** - Get suggestions tailored to your interests
- **Automated Planning** - Save time with intelligent trip organization
- **Destination Insights** - AI-powered information about destinations

## 🛠️ Tech Stack

- **Backend**: [Express.js](https://expressjs.com/) - Fast and minimal web framework
- **Database**: [MongoDB](https://www.mongodb.com/) - NoSQL document database
- **ODM**: [Mongoose](https://mongoosejs.com/) - MongoDB object modeling
- **Frontend**: [EJS](https://ejs.co/) - Embedded JavaScript templating
- **AI/ML**: Machine Learning algorithms for trip planning
- **Video Streaming**: Integration with video APIs
- **Utilities**: 
  - [ejs-mate](https://www.npmjs.com/package/ejs-mate) - EJS layout support
  - [method-override](https://www.npmjs.com/package/method-override) - HTTP method override middleware

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mayank5o4/Nestora.git
   cd Nestora
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Ensure MongoDB is running**
   ```bash
   # On macOS (if using Homebrew)
   brew services start mongodb-community

   # On Linux
   sudo systemctl start mongod

   # Or use MongoDB Atlas for cloud database
   ```

4. **Start the server**
   ```bash
   node app.js
   ```

5. **Open in your browser**
   ```
   http://localhost:8080
   ```

## 📁 Project Structure

```
Nestora/
├── app.js              # Main Express application
├── index.js            # Entry point
├── listing.js          # Listing model definition
├── data.js             # Sample data
├── package.json        # Project dependencies
├── package-lock.json   # Locked dependency versions
├── views/
│   ├── index.ejs       # Home page
│   ├── new.ejs         # New listing form
│   ├── show.ejs        # Listing detail view
│   ├── edit.ejs        # Edit listing form
│   ├── videos.ejs      # Video listings page
│   └── trip-planner.ejs # AI Trip Planner interface
└── public/             # Static assets
```

## 🚀 Usage

### Home Page
Navigate to `/` to see the home page.

### Property Listings
- **View All**: Visit `/listings` to browse all available properties
- **Create**: Go to `/listings/new` and fill in the property details
- **Details**: Click on any listing to view complete information
- **Edit**: Update property information at `/listings/:id/edit`
- **Delete**: Remove listings with the delete button

### Video Listings
- **Browse Videos**: Visit `/videos` to explore destination and property videos
- **Filter Content**: Sort videos by destination, type, or rating
- **Watch**: Stream full-length video content

### AI Trip Planner
- **Create Trip**: Visit `/trip-planner` to start planning
- **Set Preferences**: Specify your interests, budget, and duration
- **Get Itinerary**: AI generates a customized travel plan
- **View Options**: See property recommendations along with the itinerary

## 📝 API Routes

| Method | Route | Description |
|--------|-------|-------------|
| GET | `/` | Home page |
| GET | `/listings` | View all property listings |
| GET | `/listings/new` | New listing form |
| POST | `/listings` | Create new listing |
| GET | `/listings/:id` | View listing details |
| GET | `/listings/:id/edit` | Edit listing form |
| PUT | `/listings/:id` | Update listing |
| DELETE | `/listings/:id` | Delete listing |
| GET | `/videos` | View all video content |
| GET | `/videos/:id` | View specific video |
| GET | `/trip-planner` | AI Trip Planner interface |
| POST | `/trip-planner/generate` | Generate AI itinerary |

## 🔧 Environment Configuration

Update the MongoDB connection URL in `app.js`:

```javascript
const MONGO_URL = "mongodb://127.0.0.1:27017/Nestora";
```

For MongoDB Atlas:
```javascript
const MONGO_URL = "mongodb+srv://username:password@cluster.mongodb.net/Nestora";
```

## 🤝 Contributing

Contributions are welcome! Feel free to fork this project and submit pull requests for any improvements.

## 📄 License

This project is licensed under the ISC License - see the `package.json` file for details.

## 👨‍💻 Author

Created by [Mayank5o4](https://github.com/Mayank5o4)

---

**Happy Nesting! 🏡** If you find this project helpful, please consider giving it a star ⭐# Nestora
