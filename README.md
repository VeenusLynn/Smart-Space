# Smart Space 

*AI-Powered Warehouse Management System*

## 📖 Overview
Smart Space is an experimental Warehouse Management System (WMS) that combines traditional inventory tracking with AI-powered computer vision. The system can detect warehouse objects (boxes, pallets) in images, with future plans for real-time video stream processing.

### Architecture
SmartSpace/
├── smart-space-api/ (Node.js/Express backend)
├── smart-space-client/ (React frontend)
└── smart-space-detection/ (Flask AI module)


## ✨ Features
- **AI Object Detection**: YOLO model trained to recognize boxes/pallets
- **Inventory Management**: Full CRUD operations for warehouses/items
- **Role-Based Access**: Admin and staff permissions
- **Analytics Dashboard**: Visualize inventory metrics
- **Modular Design**: Independently deployable components

## 🛠️ Installation

### Prerequisites
- Node.js 16+ (for API and Client)
- Python 3.8+ (for Detection)
- MongoDB
- Redis (optional for caching)

### 1. Clone with Submodules
```bash
git clone --recursive https://github.com/VeenusLynn/SmartSpace.git
cd SmartSpace
```

### 2. Backend Setup (smart-space-api)
```bash
cd smart-space-api
npm install
cp .env.example .env  # Configure your environment variables
npm start
```

### 3. Frontend Setup (smart-space-client)
```bash
cd ../smart-space-client
npm install
npm start
```

### 4. Detection Module Setup (smart-space-detection)
```bash
cd ../smart-space-detection
python detect.py
```
