# MealPlus-DB

This is the database of my MealPlus Project

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#configuring-docker">Configuring Docker</a></li>
        <li><a href="#configuring-dbeaver">Configuring DBeaver</a></li>
      </ul>
    </li><!--
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li> -->
  </ol>
</details>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

* [Docker](https://www.docker.com/get-started) - An application for MacOS and Windows machines for the building and sharing of containerized applications.
* [DBeaver](https://dbeaver.io/) - Free multi-platform database tool for developers, database administrators, analysts and all people who need to work with databases.
* Chocolatey - Chocolatey is software management automation for Windows that wraps installers, executables, zips, and scripts into compiled packages.
  * To install execute the codes with a terminal (ex: In Windows use PowerShell):
    ```
    Get-ExecutionPolicy
    ```
    ```
    Set-ExecutionPolicy AllSigned
    ```
    ```
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
    ```
    ```
    choco
    ```
* Node.js, Yarn, Python2 e a JDK 8
  ```
  choco install -y nodejs-lts yarn python2 jdk8
  ```

### Configuring Docker

Creating container for the Data Base. With a terminal run the code below:

```
docker run --name mealplus_postgres -e POSTGRES_PASSWORD=docker2 -p 5432:5432 -d postgres
```

Verify if the container is running before executing the code
```
docker ps
```

If it is not running execute the following code, just substitue "CONTAINER_ID" for the corresponding ID that can be found with the comand above.
```
docker start "CONTAINER_ID"
```

### Configuring DBeaver
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/01.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/02.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/03.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/04.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/05.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/06.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/07.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/08.png?raw=true)
![DBeaver](https://github.com/MestreALMO/MealPlus-DB/blob/master/_README.md/DBeaver/09.png?raw=true)
<details>
  <summary>How to config with images</summary>
</details>
  
