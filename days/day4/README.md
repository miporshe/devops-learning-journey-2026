🚀 Day 4: Linux Fundamentals - First Practical Steps
📅 Date: January 14, 2026
🎯 Plan vs Reality

What I planned to do:

Study Linux file system theory

Learn permissions (chmod, chown)

Understand processes and PID

What actually happened:
✅ Explored real Linux directories (/etc, /var/log, /proc)
✅ Made permission mistakes and fixed them (755 → 600 for secrets!)
✅ Managed processes without help for the first time

💡 Key Learnings
1. Theory ≠ Practice
Reading about chmod 755 is easy. Actually seeing -rwxr-xr-x and understanding "everyone can read my secret file" — that's real learning.

2. Mistakes are the best teachers
I set wrong permissions (755) on a secret file. Fixed it to 600. This mistake taught me more than any perfect example.

3. Linux is transparent
Everything is visible: ps aux shows all processes, /proc/ exposes system internals. No black boxes here.

🛠 Technical Progress
File system exploration:

bash
# Discovered system structure
ls -la /etc/ | head -10
ls -la /var/log/
df -h  # Check disk space

# Permission practice
chmod 600 secret.txt  # Private file
chmod 755 hello.sh    # Executable script
Process management:

bash
# Run and control processes
sleep 300 &
ps aux | grep sleep
kill [PID]
