# Quick Notes: Introduction to Bash Scripting

## What is Bash Scripting?
- **Bash**: A command-line tool to interact with your computer.
- **Bash Script**: A file containing a series of commands you want the computer to execute automatically.

## Why Learn It?
- **Automate tasks**: Save time on repetitive actions.
- **Manage systems**: Handle files, software installs, and system configurations.
- **Boost efficiency**: Get more done with less typing!

---

## Getting Started
### Shebang (#!)
The first line in your script:
```bash
#!/bin/bash
```
It tells the computer to use Bash to run the script.

### Run Your Script:
1. **Make it executable**:
   ```bash
   chmod +x your_script.sh  # You learn this in the Linux Module
   ```
2. **Run it**:
   ```bash
   ./your_script.sh
   ```

---

## Basic Concepts
### Variables
Store values:
```bash
name="Ahmed"
```
Use them:
```bash
echo "Hello, $name"
```

### Comments
Add explanations with `#`:
```bash
# This line says hello
echo "Hello, World!"
```

### Conditionals
Make decisions with `if` statements:
```bash
if [ "$name" == "Alice" ]; then
  echo "Hi Alice!"
fi
```

### Loops
Repeat actions with `for` or `while`:
```bash
for i in 1 2 3; do
  echo "Number $i"
done
```

### Functions
Group commands for reuse:
```bash
greet() {
  echo "Hello, $1!"
}
greet "Alice"
```

### User Input
Get input from users:
```bash
read -p "Enter your name: " name
echo "Hello, $name!"
```

---

## Tips
- **Start small**: Write simple scripts first.
- **Use meaningful names**: This makes your script easier to understand.
- **Test often**: Avoid surprises by running your scripts frequently.

## Practice Makes Perfect!
The more you script, the better you get. Try automating small tasks daily.

**Bash scripting becomes easier with repetition—keep at it!** 🚀
