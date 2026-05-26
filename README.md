# ☁️ Cloud Portfolio Website — AWS

A personal portfolio website hosted entirely on AWS, delivered globally via a CDN, and automatically deployed through a CI/CD pipeline.

🌐 **Live URL:** https://d169sk8ak2gcsf.cloudfront.net

---

## 🏗️ Architecture

```
GitHub → AWS CodePipeline → Amazon S3 → Amazon CloudFront → Users
```

Every time code is pushed to the `main` branch, the pipeline automatically deploys the latest version to S3, which is then served globally through CloudFront.

---

## ☁️ AWS Services Used

| Service | Purpose |
|---|---|
| **Amazon S3** | Stores and hosts the static website files |
| **Amazon CloudFront** | CDN — delivers the site globally with HTTPS |
| **AWS IAM** | Bucket policy controls public read access |
| **AWS CodePipeline** | CI/CD — auto-deploys on every GitHub push |

---

## 🚀 Features

- ✅ Static website hosted on Amazon S3
- ✅ Global content delivery via CloudFront CDN
- ✅ HTTPS enabled (SSL/TLS)
- ✅ Automated deployments via CI/CD pipeline
- ✅ IAM bucket policy for secure public access

---

## 📁 Project Structure

```
my-cloud-project/
├── index.html       # Main webpage
└── style.css        # Styling
```

---

## 🔧 How It Works

1. **Storage** — Website files (`index.html`, `style.css`) are stored in an S3 bucket with static website hosting enabled
2. **Access Control** — An IAM bucket policy allows public read access to the files
3. **CDN** — CloudFront sits in front of S3, caching and serving content from edge locations worldwide with HTTPS
4. **CI/CD** — AWS CodePipeline monitors the GitHub `main` branch; any push triggers an automatic deployment to S3

---

## 📚 What I Learned

- Hosting static websites on Amazon S3
- Configuring IAM bucket policies for public access
- Setting up CloudFront distributions with HTTPS
- Building a CI/CD pipeline with AWS CodePipeline and GitHub
- Understanding CDN edge locations and cache invalidation

---

## 👤 Author

**Mahmoud Awad**
- GitHub: [@MahmoudAhmad704](https://github.com/MahmoudAhmad704)
- Email: mahmouda.dwaikat@gmail.com
