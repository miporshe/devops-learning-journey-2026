📁 Day 3: Git, GitHub, and the first push
📅 Date: January 13, 2026
🎯 Goal: Set up Git, connect SSH to GitHub, and make the first push

✅ What I did:
Set up Git globally — name and email in the config

Connected SSH — generated a key and added it to GitHub

Checked the structure — the project already has days/, scripts/, and configs/

# Push everything - first commit and push to remote repository

🛠 Commands of the day:
bash
# Setting up Git
git config --global user.name "mporse"
git config --global user.email "your_email"

# Creating and checking SSH
ssh-keygen -t ed25519
cat ~/.ssh/id_ed25519.pub # this key in GitHub

# First push
git add .
git commit -m "Day 3: Git setup and structure"
git push origin main
💡 The main takeaway:
The SSH key is my digital pass to GitHub. I no longer need to enter passwords. The entire project structure is now not only on my laptop, but also in the cloud.
