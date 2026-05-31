# CodeJudge 🚀

An interactive, full-stack algorithmic coding platform built to emulate enterprise-level remote code execution environments. 

## 🛠️ Tech Stack
* **Frontend:** React.js, Tailwind CSS
* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **Execution Engine:** C++ Child Processes

## ✨ Key Features
* **Live Code Editor:** In-browser IDE with syntax highlighting.
* **Secure Code Execution:** A custom backend engine that securely compiles and evaluates C++ submissions against hidden test cases.
* **Problem Database:** A curated database of algorithmic challenges.
* **Real-time Feedback:** Instant compilation output and error logging streamed back to the user.

## ⚙️ How the Execution Engine Works
When a user submits C++ code, the React frontend sends a payload to the Express API. The server writes this code to a temporary `.cpp` file and spawns a native C++ child process using `g++` to safely compile and run the logic against predefined inputs, returning the execution results back to the client in milliseconds.