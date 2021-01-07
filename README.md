# MealPlus-DB

This is the database of my MealPlus Project

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

<!--
## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
