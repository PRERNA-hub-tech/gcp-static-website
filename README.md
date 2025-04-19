# gcp-static-website
"Static website hosted on GCP Storage"
# Static Website Hosted on Google Cloud Storage

Welcome to my project! This is a simple static website that I’ve hosted on Google Cloud Storage (GCS). It's a great example of how to set up a static site using Google Cloud’s Object Storage services.

## 🌐 Live Website

You can view the live website by clicking the link below:
[Visit My Website](http://storage.googleapis.com/YOUR_BUCKET_NAME/index.html)

---

## 📝 Project Description

This project demonstrates how to:

- Build a static website using HTML and CSS.
- Host the website on Google Cloud Storage (GCS) for free.
- Set up a **404 error page** and a basic **index** page.

---

## 🔧 Prerequisites
    
Before you start, make sure you have the following:

- A **Google Cloud** account (sign up [here](https://cloud.google.com/)).
- Basic knowledge of **HTML** (for building web pages) and **CSS** (for styling).
- **Google Cloud Storage** to host the website.

---

## 🖥️ Project Files

Here’s what’s inside this project:


- **index.html**: This is the main page visitors will see when they first visit your website.
- **about.html**: A page to tell visitors more about your project.
- **404.html**: This page will show when someone tries to access a page that doesn't exist.
- **styles.css**: The file that makes your website look good with colors, fonts, and layout.

---

## 🚀 How to Set Up Your Own Static Website on Google Cloud

If you want to host your own website, here’s a simple guide to get started using **Cloud Shell**:

### Step 1: Create a Google Cloud Storage Bucket

1. Open **Google Cloud Console**: [https://console.cloud.google.com/](https://console.cloud.google.com/).
2. Open **Cloud Shell** by clicking the terminal icon in the top-right corner of the console.
3. Run the following command to create a **new bucket** (replace `your-unique-bucket-name` with your desired bucket name):

### 
gsutil mb gs://your-unique-bucket-name

### To make the bucket publicly accessible, run:
gsutil iam ch allUsers:objectViewer gs://your-unique-bucket-name

# Enable website hosting on the bucket by setting the index.html as the Main Page and 404.html as the Error Page:
gsutil web set -m index.html -e 404.html gs://your-unique-bucket-name

### Step 2: Upload Your Files to Google Cloud Storage

1. In the Google Cloud Console, go to **Storage** > **Browser**.
2. Click your bucket name.
3. Click **Upload Files** and upload your HTML and CSS files (like `index.html`, `about.html`, etc.).
  
# Access Your Website
http://storage.googleapis.com/your-unique-bucket-name/index.html

Just replace your-unique-bucket-name with the name of your actual bucket.

---

## 🛠️ Technologies Used

- **HTML**: Used to structure the content of the web pages.
- **CSS**: Used to style the pages and make them visually appealing.
- **Google Cloud Storage (GCS)**: Used to host the static website and manage files.
- **GitHub**: Used for version control to track and manage changes to the project.

---

## 📄 Additional Resources

- [Google Cloud Storage Documentation](https://cloud.google.com/storage)
- [Learn HTML](https://www.w3schools.com/html/)
- [Learn CSS](https://www.w3schools.com/css/)




