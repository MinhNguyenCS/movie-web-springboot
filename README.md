# 🎥 Anime Streaming Website

![Anime Streaming Banner](https://your-image-link.com/banner.jpg)

Welcome to the **Anime Streaming Website**! This project is a **full-stack anime streaming platform** where users can **browse anime by category** and **search for anime by name**. Built using **Java Spring Boot**, **MongoDB**, and **HTML/CSS/JavaScript**, this application ensures smooth performance and scalability. 🚀

## 🌟 Features
- 📌 **Display anime by category** (e.g., Action, Romance, Adventure, Comedy, etc.)
- 🔍 **Search for anime by name**
- 📺 **Stream anime episodes**
- 🎨 **User-friendly UI**
- ⚡ **Fast and optimized performance**

## 🛠️ Tech Stack
### **Backend** (🔧)
- 🖥️ **Java Spring Boot**
- 🗄️ **MongoDB (via Docker)**
- 🔐 **JWT Authentication (optional)**

### **Frontend** (🎨)
- 🌐 **HTML, CSS, JavaScript**
- 📜 **Fetch API for dynamic content loading**
- 📲 **Responsive Design**

## 🚀 Getting Started

### **1️⃣ Clone the Repository**
```bash
 git clone https://github.com/yourusername/anime-streaming.git
 cd anime-streaming
```

### **2️⃣ Setup the Backend**
1. Install **Java (17 or above)** and **Maven**.
2. Update `application.properties` with your MongoDB connection details.
3. Run the backend:
```bash
 mvn spring-boot:run
```

### **3️⃣ Setup the Frontend**
1. Navigate to the frontend directory:
```bash
 cd frontend
```
2. Open `index.html` in a browser or use **Live Server**.

## 🐳 Running MongoDB with Docker
To run MongoDB in a **Docker container**, use:
```bash
docker run -d -p 27017:27017 --name mongo-db mongo
```

## 🌍 Deployment on EC2
1. **Build the Backend**:
```bash
 mvn clean package
```
2. **Run with Docker**:
```bash
docker run -d -p 443:8085 \
--restart always \
-e SPRING_DATA_MONGODB_DATABASE=movie-api-db \
-e SPRING_DATA_MONGODB_URI=mongodb+srv://your-db-connection-string \
-e SERVER_SSL_KEY_STORE=classpath:keystore.jks \
-e SERVER_SSL_KEY_STORE_PASSWORD=password \
-e SERVER_SSL_KEY_ALIAS=myapp \
-e SERVER_SSL_KEY_PASSWORD=password \
--name anime-backend your-docker-image
```
3. **Access the Site:** Open `https://your-ec2-ip/` in a browser.

## 📸 Screenshots
### **Homepage**
![Homepage](https://your-image-link.com/homepage.jpg)

### **Anime Categories**
![Categories](https://your-image-link.com/categories.jpg)

### **Search Functionality**
![Search](https://your-image-link.com/search.jpg)

## 🤝 Contributing
Want to contribute? Feel free to submit a pull request! 🚀

## 📜 License
This project is licensed under the **MIT License**.

## 💬 Contact
- **GitHub:** [YourUsername](https://github.com/yourusername)
- **Website:** [Your Website](https://yourwebsite.com)

---

_Enjoy watching anime! 🎥✨_

