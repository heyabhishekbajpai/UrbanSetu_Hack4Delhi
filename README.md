# UrbanSetu - Civic Issue Reporting Platform

> **आवाज़ उठाओ, बदलाव लाओ** (Raise Your Voice, Bring Change)

<!-- FORCE VERCEL DEPLOYMENT - Version 1.2.0 - Supabase Integration & Admin Features -->

A modern, AI-powered civic issue reporting and resolution platform designed for mobile-first usage. UrbanSetu connects citizens with local authorities for faster, more efficient problem-solving through crowdsourced reporting and real-time tracking.

## 🌟 Features

### For Citizens
- **AI-Powered Issue Detection**: Automatically identify civic issues using Teachable Machine
- **Quick Reporting**: Mobile-optimized camera capture and form submission
- **Interactive Maps**: GPS-based location capture with reverse geocoding
- **Real-time Tracking**: Monitor complaint progress from submission to resolution
- **Smart Routing**: Automatic department assignment based on AI detection
- **Secure Authentication**: Email, Google, and Phone login options

### For Administrators
- **Live Dashboard**: Comprehensive overview of all complaints and statistics
- **Detailed Complaint View**: In-depth analysis of individual complaints with status updates
- **Priority Map**: Color-coded map markers (Red/Orange/Yellow/Green) for urgent issues
- **Role-Based Access**: Secure admin verification via Supabase RLS
- **Department Analytics**: Performance metrics and response time tracking

### Technical Features
- **Supabase Backend**: Robust database, authentication, and storage
- **Row Level Security (RLS)**: Data privacy and secure access control
- **Mobile-First Design**: Optimized for smartphones and tablets
- **Dark/Light Mode**: User preference support
- **Real-time Updates**: Live status notifications
- **Image Processing**: AI-powered civic issue classification

## 🚀 Tech Stack

- **Frontend**: React.js 18 with modern hooks
- **Backend**: Supabase (PostgreSQL, Auth, Storage)
- **Styling**: Tailwind CSS with custom components
- **Icons**: Lucide React
- **Animations**: Framer Motion
- **Maps**: Leaflet.js & OpenStreetMap
- **AI/ML**: TensorFlow.js with Teachable Machine
- **State Management**: React Context API
- **Routing**: React Router DOM
- **Forms**: React Hook Form
- **Notifications**: React Hot Toast
- **Date Handling**: date-fns

## 🎨 Design System

### Color Scheme
- **Light Mode**: Green (#2d5016, #48bb78) and white with subtle gradients
- **Dark Mode**: Dark green (#1a3d0a) and grey (#2d3748)

### UI Components
- Glassmorphism effects for modern aesthetics
- Smooth animations and micro-interactions
- Professional civic app design language
- Mobile-first responsive layouts

## 🤖 AI Integration

### Teachable Machine Model
- **Model Location**: Local files in `/public/models/` directory
- **Model Files**: model.json, metadata.json, model.weights.bin
- **Classes**: Pothole, Garbage, Sewage, StreetLight, FallenTree
- **Confidence Threshold**: >60% for auto-selection
- **Manual Override**: Available for low-confidence predictions

### Department Mapping
- **Pothole** → Road Authority
- **Garbage** → Sanitation Department
- **Sewage** → Water & Sewage Board
- **StreetLight** → Electrical Department
- **FallenTree** → Parks & Horticulture

## 🛠️ Installation & Setup

### Prerequisites
- Node.js 16+ and npm
- Modern web browser with camera access
- Internet connection for AI model loading
- Supabase Project Credentials

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd urbansetu
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment Variables**
   Create a `.env` file in the root directory and add your Supabase credentials:
   ```env
   REACT_APP_SUPABASE_URL=your_supabase_url
   REACT_APP_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. **Start development server**
   ```bash
   npm start
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

## 📱 Application Structure

### Public Pages
- **Landing Page**: Hero section, features, testimonials, and call-to-action
- **Authentication**: Login/Register with Citizen/Admin options
- **Social Login**: Google OAuth and phone number support (Citizen only)

### Citizen Dashboard
- **Quick Report**: One-tap issue reporting with camera integration
- **Recent Complaints**: Status timeline and progress tracking
- **Statistics**: Personal reporting metrics
- **Profile Management**: Account settings and preferences

### Admin Dashboard
- **Live Map View**: Geographic complaint visualization with priority indicators
- **Complaints Table**: Filterable and searchable complaint management
- **Detailed View**: Manage individual complaints and update status
- **Analytics**: Department-wise performance metrics

## 🔒 Security & Roles

- **Citizens**: Can report issues and view only their own complaints.
- **Admins**: Can view all complaints, update status, and access analytics.
- **RLS Policies**: Enforced at the database level to prevent unauthorized access.
- **Admin Verification**: UI checks for 'admin' role in `profiles` table.

## 🚀 Deployment

### Build Process
```bash
npm run build
```

### Deployment Options
- **Netlify**: Drag and drop the build folder
- **Vercel**: Connect GitHub repository
- **AWS S3**: Upload build files to S3 bucket
- **Heroku**: Deploy with buildpacks

## 📞 Support

For support and questions:
- **Email**: bajpai.connect@gmail.com

---

**Made with ❤️ for better cities and communities**

*UrbanSetu - Empowering citizens to build better cities, one report at a time.*
