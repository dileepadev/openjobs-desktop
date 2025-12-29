# OpenJobs Desktop Appilcation

![GitHub repo size](https://img.shields.io/github/repo-size/dileepadev/openjobs-desktop?color=red&label=repository%20size)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/dileepadev/openjobs-desktop?color=red)
![GitHub language count](https://img.shields.io/github/languages/count/dileepadev/openjobs-desktop)
![GitHub top language](https://img.shields.io/github/languages/top/dileepadev/openjobs-desktop)
![GitHub](https://img.shields.io/github/license/dileepadev/openjobs-desktop?color=yellow)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/dileepadev/openjobs-desktop?color=brightgreen&label=commits)

## ✨ About

The **OpenJobs Desktop Appilcation** helps to manage data congestion and find the best low-data traffic services. This concept is built on data structures. This alpha release does not include the complete requirements and interface. **This project has been developed as an open source for educational purposes.**

![Preview Image](https://dileepadev.github.io/images/openjobs-desktop/preview.png)

## 🎞️ Demo Video

Click the link or image below to view the demo video on YouTube.

🔗 <https://youtu.be/oRQKSB9skfA>

[![Watch the demo video](https://img.youtube.com/vi/oRQKSB9skfA/0.jpg)](https://youtu.be/oRQKSB9skfA)

## 📦 Release Details

Release Version - 1.0.0  
Initial release date - October 19, 2020

> [!NOTE]
> This repository is a clean re-upload to my new GitHub account. No new features or functionality have been added. Minor compatibility fixes may have been applied to ensure the project runs correctly in the current environment. Please note that the original commit history from the previous account is not preserved. This update is primarily for migration purposes.
>
> **Initial release date:** October 19, 2020  
> **Migration date:** December 28, 2025  

## 💡 Deployment

Deployment is not currently in use

## 💻 Built with

- Java 8 (jdk-8u461-windows-i586d)
- Java 25 (Compatible version)
- Java Swing
- NetBeans 8.2 (Development IDE)
- Apache NetBeans 28 (Compatible IDE)
- SQL Database
- Data Structures

## 📌 Prerequisites

Before you get started, follow these requirements

- Java JDK 8
- NetBeans 8.2 or Apache NetBeans 28
- WampServer or XAMPP is good for localhost
- phpMyAdmin database

## 🍃 How to Setup

- Download or clone the repository
- Move the project to the selected directory
- Clean and build project
- Use application to create the database

## 🚀 How to Run

- Clean and build the project
- Connect database and localhost
- Run the project
- Select the "Issue? Click here" option, then select the "Database Create" option to create the database

## 🚪 How to open

Before you start

- Ensure your local web server (WampServer or XAMPP) is running and phpMyAdmin is available.
- On first run, create the application's database (see "Create the database" below).

Create the database

1. Launch the application.
2. From the menu choose "Issue? Click here" → "Database Create".
3. Follow the on-screen instructions and verify the new database in phpMyAdmin.

Run options

- As a NetBeans project: open the `OpenJobs` project folder, then select **Clean and Build** before running.
- As a native executable: run `Setup/OpenJobs.exe` from the Setup Files.
- As a jar: run `Setup/OpenJobs.jar` with `java -jar OpenJobs.jar`.

Login

- After creating the database, retrieve the initial User ID and Password using phpMyAdmin.
- Use those credentials to sign in to the application.

Search files

- For the Transfer panel's search feature, use `openjobs_locations.txt` as the template.

***IMPORTANT: Always run "Clean and Build" in your IDE before launching the project. The application may not run correctly otherwise.***

## 🧱 Application Structure

It uses 3 main user services and server services speed = 3 < 1 < 2

1. Server Services 1 = Receive Servers
   - Use Grapth Theory: Path Weighted Dijkstra's algorithm
   - Use Database Table: path_weighted
   - Use Vertex: 6
   - Path weight changes
   - Input source for find the minimum traffic between servers
   - Receive projects by minumum traffic server path
   - Admins can manage paths weight
   - Paths cannot change
   - Each vertex has 2 connections with 2 different vertex  

2. Server Services 2 = Send Servers
   - Use Grapth Theory: Path Unweighted Dijkstra's algorithm
   - Use Database Table: path_unweighted
   - Use Vertex: 10
   - Vertext connection changes
   - Input source and destination for find the shortest lenghth
   - Send projects by shortest traffic server path
   - Admins can manage paths connection  

3. Server Services 3 = Filter Projects, View Status, Transfer
   - Filter Projects
     - Use Sorting Algorithm: Quick Sort
     - Use Database Table: project
     - Filter by remaining project days
   - View Status
     - Use for view all summary and server health
     - Notify about upcoming projects
     - Use Database Table: upcoming_projects
   - Transfer
     - Use for view locations to transfer
     - This panel is under development

## 📸 Icons and Images

- Icons8 - <https://icons8.com>
- Freepik - <https://www.freepik.com>
- unDraw - <https://undraw.co>

## ❤️ Thanks

Thanks to everyone who supported

## 👨‍💻 Developed By

Dileepa Bandara  
[@dileepadev](https://github.com/dileepadev)  
<https://dileepa.dev>

> [!NOTE]
> This repository may contain references to my former GitHub username (`dileepadev`) and domain (`dileepadev.dev`), which I no longer use. These identifiers may now belong to other parties. All current development and maintenance are conducted under my new GitHub account [dileepadev](https://github.com/dileepadev) and domain [dileepa.dev](https://dileepa.dev).

## 💬 Contact

If you want to contact me, leave a message via email.

- Email - <contact@dileepa.dev>

## 📜 License

This project is licensed under the MIT License.  
See the license file for more details [LICENSE.md](./LICENSE)
