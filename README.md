CCC181 Laboratory 1
Personal Portfolio Landing Page

Student: Prinze June Rey E. Tingson
Course: CCC181

1. Introduction

This laboratory activity focuses on creating a personal portfolio landing page using HTML and CSS and integrating it with the Bonezegei Scripting Language (BSL) HTTP server framework. The portfolio presents the student's profile, skills, projects, achievements, contact information, and social links.

2. Objectives

Create a personal portfolio landing page.

Use HTML to structure webpage content and CSS to style the layout.

Configure and run a local BSL HTTP server.

Organize project files in Visual Studio Code.

Document the setup, workflow, and testing results.

Prepare the project for publication on GitHub.

3. Development Environment

Tool / Technology

Purpose

Visual Studio Code

Editing and organizing project files

Bonezegei Scripting Language (BSL)

Running the HTTP server

HTML

Structuring portfolio content

CSS

Styling and responsive layout

PowerShell

Running commands and checking files

GitHub

Hosting source code and version control

4. Project Structure

The project is organized with the server script and package configuration in the root directory, the HTTP library in the lib folder, and the website files in public.

BSL_HTTP_and_WebSocket-main/
├── app.bzg
├── package.json
├── README.md
├── LICENSE
├── lib/
│   ├── http.bzg
│   ├── http.json
│   └── http/http.dll
└── public/
    ├── index.html
    └── 404.html

5. Setup and Workflow

Download and open the project

The BSL HTTP and WebSocket project was downloaded and extracted. In Visual Studio Code, File → Open Folder was used to open the project directory.

Verify BSL

The terminal command `bonezegei --version` reported Bonezegei Script Interpreter v1.3.3 on Windows.

Install dependencies

The command `bzg install` was executed in the project root. The terminal reported that the HTTP package was installed for arch=x86.

Configure the server

The app.bzg file includes the HTTP library with `include("lib/http.bzg");` and initializes the server using `var server = http(8000);`. The GET handler serves public/index.html for the root path and public/404.html for other paths.

Run the server

The command `bzg run` was used to launch the project. During testing, the HTTP native library failed to load, so the server did not start successfully.

View the portfolio

The portfolio screenshot included in this report shows the page opened in Chrome from a local file path. For final server verification, open http://localhost:8000 after the BSL HTTP library issue is fixed.

6. Portfolio Website Features

Full Name and Profile Summary: Introduces the student and provides a short profile summary.

Skills and Technologies: Lists skills and technologies relevant to the student's studies and projects.

Projects and Achievements: Highlights projects, laboratory activities, and achievements.

Contact Information and Social Links: Provides contact details and links to social media or professional profiles.

7. Screenshot Evidence

Screenshot 1: Terminal Output (bzg run)

During testing, the terminal displayed the following error: “Failed to load library: lib/http/http.dll” followed by “Undefined variable http.” This indicates that the native HTTP library did not load, preventing the server from starting. The terminal screenshot should be inserted here as troubleshooting evidence.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d98569d5-276d-40d3-a4aa-360c972472cc" />
Screenshot 2: Browser Rendering

The screenshot below shows the personal portfolio landing page rendered in Google Chrome. It includes a navigation bar, profile photo, name and profile summary, student information, and a button to explore the portfolio.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0178802d-ca43-4e3e-a067-01952f27e08e" />

