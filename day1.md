🎯 LEVEL 1 — BASIC QUESTIONS (VERY COMMON)
❓ What is Linux?

👉 Expected:

Linux is an operating system used in servers, and it’s mostly operated via terminal commands.

❓ Difference between cd, ls, and pwd?

👉 Expected:

cd → change directory
ls → list files
pwd → show current path
❓ How do you create and delete files/folders?

👉 Commands:

mkdir folder
touch file.txt
rm file.txt
rm -r folder
❓ Difference between rm and rmdir?

👉 Expected:

rmdir → only empty folders
rm -r → folders with content

🎯 LEVEL 2 — PRACTICAL QUESTIONS
❓ How do you copy a file from one folder to another?

👉 Example:

cp app/config/app.conf backup/app.conf.bak

👉 They want to see:

You understand paths
You can rename while copying
❓ What is the difference between > and >>?

👉 Expected:

> → overwrite
>> → append
❓ How do you make a file executable?
chmod +x script.sh
❓ What is mkdir -p?

👉 Expected:

It creates nested directories and avoids errors if parent folders don’t exist.

🎯 LEVEL 3 — DEBUGGING (VERY IMPORTANT)
❓ How do you check logs?

👉 Expected:

less file.log
tail file.log
❓ How do you monitor logs in real time?
tail -f file.log
❓ How do you find errors in logs?
grep "ERROR" file.log
❓ How do you see only latest errors?
tail -f file.log | grep ERROR

💥 This answer impresses interviewers

❓ How do you count errors in logs?
grep "ERROR" file.log | wc -l
🎯 LEVEL 4 — SCENARIO QUESTIONS (MOST IMPORTANT)
❓ “Your application is not working. What will you do?”

👉 Expected answer:

First, I will check logs using tail -f or less.
Then I will search for errors using grep.
Based on errors, I will debug the issue.

❓ “You ran a command and nothing is happening (like tail -f). What’s going on?”

👉 Expected:

It’s a continuous process running in foreground. I can stop it using Ctrl + C.

❓ “File not found error — how do you debug?”

👉 Expected:

Check current directory → pwd
Check files → ls
Verify path
🎯 LEVEL 5 — TRICK QUESTIONS
❓ What happens if you run:
rm -rf /

👉 Expected:

It deletes entire system (very dangerous)

❓ Why did cd.. not work?

👉 Expected:

Because Linux requires space → cd ..

❓ Difference between relative and absolute path?

👉 Expected:

Relative → from current directory
Absolute → full path from root
🧠 WHAT INTERVIEWERS ARE REALLY CHECKING

They don’t care if you memorize commands.

They care if you:

Think logically ✅
Debug errors ✅
Understand system behavior ✅
🔥 HOW TO ANSWER LIKE A PRO

Instead of just saying:

“Use grep”

Say:

“I would check logs and filter errors using grep to quickly identify issues”

👉 Shows thinking, not memorization
