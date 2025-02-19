## Step 1: Duplicate this repository (including the issues)

By the end of this process, you will:
- Understand how to manage repositories on GitHub.
- Learn how to use issues, labels, and milestones for tracking progress.
- Gain hands-on experience with Node.js scripts and API automation.

Your first assignment is to **duplicate this repository** into a new public repo where you will track your progress.

---

## ✅ **How to Duplicate This Repository**
Follow these steps carefully to set up your own intern repository.

### **1️⃣ Create a New Public Repository**
1. Go to [GitHub](https://github.com/).
2. Click on **New Repository**.
3. Name it something like `your-username-intern-repo`.
4. **Set it to Public** (so we can review it).
5. **Initialize with a README and MIT License**.
6. Copy the new repository URL.

### **2️⃣ Create a GitHub Personal Access Token**
To allow the script to create issues, labels, and milestones, you need to generate a **fine-grained personal access token**.

#### **Steps to Generate a Token:**
1. Go to **[GitHub → Settings → Developer Settings → Personal Access Tokens](https://github.com/settings/tokens)**.
2. Click on **"Generate new token (fine-grained)"**.
3. Call it something like "Clone Focus Bear onboarding repo"
4. Set the following **permissions**:
   - **Repository Access:** Select **"Select repositories"** and choose **only your new repository**.

![CleanShot 2025-02-15 at 08 38 42](https://github.com/user-attachments/assets/3b9b8caa-b710-4706-bb53-b3d846f2de7e)


   - **Permissions:**
     - Issues → **Read and Write**
     - Metadata → **Read**
    
![CleanShot 2025-02-15 at 09 00 34](https://github.com/user-attachments/assets/3e1a7178-95ea-44a9-9f5f-3baaafc76a7a)


5. Click **Generate Token** and copy the token (you won’t see it again!).

---

### **3️⃣ Clone This Repository**
Download the source repository to your local machine:
```sh
 git clone https://github.com/Focus-Bear/onboarding-frontend-react.git
 cd onboarding-frontend-react
```

### **4️⃣ Run the Script to Duplicate Issues, Labels, and Milestones**

#### **Go to the `duplicate-repo` Folder**
```sh
cd duplicate-repo
```

#### **Install Dependencies**
```sh
npm install
```

#### **Create a `.env` File**
1. Copy the example file:
   ```sh
   cp .env.example .env
   ```
2. Open `.env` and edit the following:
   ```ini
   GITHUB_TOKEN=your_github_token_here
   SOURCE_REPO=Focus-Bear/onboarding-frontend-react
   DEST_REPO=your-username-intern-repo
   ```
   - Replace `your_github_token_here` with your **GitHub Personal Access Token**.
   - Replace `your-username-intern-repo` with your **new repository name**.

#### **Run the Script**
```sh
node duplicateRepo.js
```
This will **copy all issues, labels, and milestones** into your new repository.

### **5️⃣ Verify Your Repository**
1. Go to your new repository on GitHub.
2. Check that:
   - Issues have been copied ✅
   - Labels exist ✅
   - Milestones are present ✅

### **6️⃣ Start Working on Issues!**
- Now that your repository is set up, you can start working through the issues.
- **Ask for help** if you run into problems! We’re here to support you. 😊

---

## ❓ Troubleshooting
- **GitHub API rate limit exceeded?**
  - Wait a few minutes or generate a new token with higher rate limits.
- **Issues/labels not appearing?**
  - Check the script output and ensure `.env` values are correct.
- **Script not running?**
  - Run `node -v` to check if Node.js is installed.

📢 If you're still stuck, **reach out in Discord!** 🎯

---

## 🎉 Congratulations!
You have successfully set up your own project repository! Now, move on to your first assigned issue and get started. 🚀
