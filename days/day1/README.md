# 🚀 Day 1: Choosing the infrastructure and the first steps
## 📅 Date: January 11, 2026

## 🎯 Plan vs reality

### What I thought I would do:
- Install the "right" Linux through VirtualBox
- Have a full-fledged Ubuntu GUI
- Follow the "standard" learning path

### What actually happened:
✅ **Tried VirtualBox + Ubuntu Desktop** - the laptop couldn't handle it 
✅ **Explored alternatives** — found WSL2 
✅ **Installed WSL2 with Ubuntu 24.04 LTS** — it worked! 
✅ **Saw my first Linux terminal** — a small victory!

## 💡 Discoveries of the day

### 1. Tools should help, not hinder
While trying to make VirtualBox work, I realized the most important thing: 
**The right tool is the one that solves a problem, not creates new ones.** 
WSL2 wasn't a "blanket" - it was a smart choice for my hardware.

### 2. Simplicity can be professional
In Russian-speaking IT, people often think that "complex = professional". 
It turned out that **Microsoft engineers themselves use WSL2**. 
If it suits them, it's definitely suitable for a beginner DevOps.

### 3. The terminal is the beginning of the journey
When I finally saw it:
It wasn't just an input line. It was the **moment when "learning DevOps" became "doing DevOps"**.

## 🛠 Technical steps

### How I installed the environment:
```powershell
# In Windows PowerShell (as an administrator)
wsl --install -d Ubuntu
# I waited for 2 minutes... and it worked!
