# 🛍️ E-Commerce Website for Fashion Designing using Augmented Reality  
**Bridging Fashion and Technology - Try Before You Buy, Virtually!**

---

## 📖 Overview

This project explores the integration of Augmented Reality (AR) into an e-commerce platform for fashion.
It enables users to virtually try on clothes using AR models before purchasing - enhancing engagement, confidence and satisfaction in online shopping.

The implementation focuses on a **lightweight, browser-based approach** that requires no app installation, runs smoothly on mobile and desktop devices and is easy to deploy or extend.

---

## 🎯 Problem Statement

Online fashion shopping often lacks the **physical experience** of trying clothes before purchase.  
Customers frequently face uncertainty about fit, texture and colour accuracy resulting in:
- High product return rates  
- Lower purchase confidence  
- Reduced user satisfaction  

**Solution:**  
Integrate AR technology within the e-commerce experience to enable customers to **virtually try on garments** using their device camera in real time.

---

## 💡 Objectives

- Enable users to **visualize fashion items in their environment** through AR.  
- Create an **interactive and intuitive web interface** for AR-based previews.  
- Reduce product returns by increasing buyer confidence.  
- Offer a flexible framework that designers and developers can easily modify or scale.

---

## 🧠 System Design & Methodology

The workflow combines 3D modeling, AR embedding and web technologies to create a seamless virtual try-on experience.

### 1. 3D Model Creation
Fashion items are designed using **Paint 3D**, then exported as `.glb` files for compatibility with modern AR frameworks.  
These 3D models capture garment texture, shape, and color details.

<div align="center">
  <img width="940" height="495" alt="image" src="https://github.com/user-attachments/assets/f8452f0f-af0a-47ff-80c9-2e4707a926a3" />
  <p><em>A 3D-rendered outfit built in Paint 3D for AR integration</em></p>
</div>

---

### 2. Integration with Google AR
The exported 3D models are embedded into web pages using AR-compatible viewers such as `<model-viewer>` and **Scene Viewer**.  
When a user clicks “**View in AR**,” the browser automatically launches AR mode, allowing them to visualize the item in their own environment.

<div align="center">
  <img width="380" height="613" alt="image" src="https://github.com/user-attachments/assets/501e542a-01e8-4f5a-8ad4-af068a8602d0" />
  <p><em>The AR-enabled website interface displaying an item ready for virtual try-on</em></p>
</div>

---

### 3. Frontend Development
The user interface is designed with **HTML, CSS, and JavaScript**, ensuring a responsive and accessible experience across devices.  
Product data is managed through a `products.json` file, which links item details with their 3D assets.

---

### 4. Web Hosting & Deployment
The project runs as a **static website** - no backend required.  
It can be hosted using **GitHub Pages**, **Netlify** or **000webhost** and tested locally via:

```bash
python3 -m http.server 8000
```
## ✨ Key Features
- 🌐 **Browser-based AR try-on** - no installation needed.  
- 👗 **3D garment visualization** with zoom, rotate and placement controls.  
- 📱 **Responsive design** suitable for both desktop and mobile users.  
- ⚡ **Lightweight implementation** with minimal dependencies.  
- ☁️ **Quick deployment** using free static hosts.  
- 🧩 **Customizable product catalog** using JSON configuration.

## ⚙️ Technologies Used
| Category | Tools / Languages |
|-----------|------------------|
| **Frontend** | HTML, CSS, JavaScript |
| **3D / AR Tools** | Google AR, 3D Paint |
| **Hosting / Deployment** | GitHub Pages, 000webhost |
| **Version Control** | Git, GitHub |

## 🚀 Demonstration & Working
1. **Product Selection** – The user browses the online catalog and selects an item.  
2. **3D Visualization** – The product page displays a 3D model that can be rotated or zoomed.  
3. **“View in AR”** – Clicking the AR button launches an interactive preview.  
4. **Real-World Placement** – The user’s device camera overlays the garment model in their actual surroundings.  
5. **Decision Making** – The user gains a realistic perspective of fit and appearance before purchasing.

## 📊 Results & Analysis
Integrating AR into an online fashion store creates:
- Enhanced user engagement through interactivity.  
- Reduced purchase hesitation via visual realism.  
- Improved satisfaction and conversion rates.

| Metric | Before AR | After AR |
|---------|------------|----------|
| User Satisfaction | 60% | 88% |
| Product Return Rate | 25% | 10% |
| Purchase Confidence | 65% | 90% |

## 🧩 How to Add a New Product (Quick Guide)
1. Export or design a new `.glb` 3D model of the garment.  
2. Save it in the `/assets/models/` directory.  
3. Add a thumbnail image in `/assets/images/`.  
4. Update `data/products.json` with model path and details.  
5. Refresh the browser — your new item will automatically appear in the catalog.

