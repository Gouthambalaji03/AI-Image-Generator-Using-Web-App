# AI Image Generation App - MERN Stack

A full-stack MERN application that generates AI images using DALL-E and allows users to share them with the community.

![AI Image Generation App]

## 🚀 Features

- **AI Image Generation**: Create stunning images using OpenAI's DALL-E API
- **Community Sharing**: Share your generated images with other users
- **Search Functionality**: Search through all shared images by name or prompt
- **Responsive Design**: Modern UI built with React and Tailwind CSS
- **Real-time Updates**: See new images as they're shared by the community

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI framework
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **React Router** - Navigation

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB

### External APIs
- **OpenAI DALL-E** - AI image generation
- **Cloudinary** - Image storage and hosting

## 📋 Prerequisites

Before running this project, make sure you have:

- **Node.js** (version 14 or higher)
- **npm** or **yarn** package manager
- **MongoDB** (local installation or MongoDB Atlas account)
- **OpenAI API Key** (for DALL-E image generation)
- **Cloudinary Account** (for image storage)

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd project_ai_mern_image_generation-main
```

### 2. Set Up Environment Variables

Create a `.env` file in the `server` directory:

```env
# MongoDB Connection String
MONGODB_URL=mongodb://localhost:27017/dalle_db

# OpenAI API Key (for DALL-E image generation)
OPENAI_API_KEY=your_openai_api_key_here

# Cloudinary Configuration (for image storage)
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### 3. Get Your API Keys

#### OpenAI API Key
1. Go to [OpenAI Platform](https://platform.openai.com/api-keys)
2. Sign up or log in to your account
3. Create a new API key
4. Copy the key and add it to your `.env` file

#### Cloudinary Credentials
1. Go to [Cloudinary](https://cloudinary.com/) and create an account
2. Navigate to your Dashboard
3. Copy your Cloud Name, API Key, and API Secret
4. Add them to your `.env` file

#### MongoDB Setup
**Option A: Local MongoDB**
- Install MongoDB locally
- Use connection string: `mongodb://localhost:27017/dalle_db`

**Option B: MongoDB Atlas (Recommended)**
1. Go to [MongoDB Atlas](https://www.mongodb.com/atlas)
2. Create a free cluster
3. Get your connection string
4. Replace `<password>` with your database password

### 4. Install Dependencies

**Install server dependencies:**
```bash
cd server
npm install
```

**Install client dependencies:**
```bash
cd client
npm install
```

### 5. Run the Application

**Start the server (Terminal 1):**
```bash
cd server
npm start
```
The server will run on `http://localhost:8080`

**Start the client (Terminal 2):**
```bash
cd client
npm run dev
```
The client will run on `http://localhost:5173`

### 6. Access the Application

Open your browser and navigate to `http://localhost:5173`

## 📖 Usage

### Generating Images
1. Click the "Create" button in the header
2. Enter your name and a detailed prompt describing the image you want
3. Click "Generate" to create the image using DALL-E
4. Once satisfied, click "Share with the Community" to save it

### Browsing Images
1. The home page shows all images shared by the community
2. Use the search bar to find specific images by name or prompt
3. Images are displayed in a responsive grid layout

### Tips for Better Prompts
- Be specific and descriptive
- Include style preferences (e.g., "oil painting", "digital art", "photography")
- Mention lighting, mood, and composition details
- Use the "Surprise Me" button for random creative prompts

## 🏗️ Project Structure

```
project_ai_mern_image_generation-main/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── page/          # Page components
│   │   ├── assets/        # Static assets
│   │   ├── constant/      # Constants and configurations
│   │   └── utils/         # Utility functions
│   └── package.json
├── server/                 # Backend Node.js application
│   ├── routes/            # API route handlers
│   ├── mongodb/           # Database models and connection
│   └── package.json
└── README.md
```

## 🔌 API Endpoints

### DALL-E Routes (`/api/v1/dalle`)
- `POST /` - Generate image from prompt

### Post Routes (`/api/v1/post`)
- `GET /` - Fetch all posts
- `POST /` - Create new post

## 🐛 Troubleshooting

### Common Issues

**"Failed to fetch" Error**
- Ensure the server is running on port 8080
- Check that all environment variables are set correctly
- Verify your API keys are valid

**MongoDB Connection Issues**
- Check your MongoDB connection string
- Ensure MongoDB is running (if using local installation)
- Verify network connectivity (if using MongoDB Atlas)

**Image Generation Fails**
- Verify your OpenAI API key is correct and has sufficient credits
- Check that your prompt follows OpenAI's content policy
- Ensure you have a stable internet connection

**Image Upload Issues**
- Verify your Cloudinary credentials are correct
- Check that your Cloudinary account is active

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [OpenAI](https://openai.com/) for providing the DALL-E API
- [Cloudinary](https://cloudinary.com/) for image storage services
- [MongoDB](https://www.mongodb.com/) for the database
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework

## 📞 Support

If you encounter any issues or have questions:

1. Check the troubleshooting section above
2. Review the console logs for error messages
3. Ensure all dependencies are properly installed
4. Verify your environment variables are correctly set

---

**Happy Image Generating! 🎨✨**
