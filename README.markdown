# Resume Host

## Purpose

**(Windows Only)**  
Step-by-step procedure of hosting a portfolio online using Jekyll Static Generator so that multiple  
employers can easily check through and the resume can be updated anytime

### Prerequisites

Requird Softwares:

```
Markdown Editor
Ruby
Google Chrome Browser
Github
```

### Instructions

1. Markdown editor

    Use a [markdown editor](https://www.readme.so/editor)  
    And download the resume in markdown format  
    EXAMPLE:

    ```
    README.md
    ```
2. Install Ruby

    latest version of Ruby from the [website](https://rubyinstaller.org/downloads/)
    Use cmd to check if Ruby is installed or not by typing the following commands
    ```console
    ruby -v
    gem -v
    ```
    ![Ruby Install](https://github.com/AhirGit/Jekyll_Portfolio/raw/comp3040A2_pages/Ruby%20installation.gif)

3. Install gem package manager and Jekyll using the following cmd commands

    ```console
    gem install jekyll bundler
    ```
    Use cmd to check if Jukyll is installed or not by typing the following commands
    ```console
    jekyll -v
    ```
4. Create a Jekyll site

    Change current directory to the host directory and run the following  
    cmd command to create the local host for the site
    ```console
    jekyll new directory_name
    ```
    Site has been created sucessfully
5. Host your resume written in markdown
    ```
    Copy and paste your markdown code in  
    directory_name/index.markdown
    ```
    At the very top of your markdown code input the code
    ```markdown
    ---
    layout: home
    title: "Resume"
    ---
    ```
    to make sure the resume is in the first page of the site
6. Push to GitHub repository  
   **(Make sure you have a [GitHub Account](https://github.com/) and [GitHub Installed](https://git-scm.com/downloads)** in Windows  
   ```markdown
   - Click new repository in Github
   - Name the repository similar to the directory_name
   - Open config.yml
   - Change baseurl: "" to baseurl: "directory_name"
   - Use cd to make directory_name the current directory
   ```
   Type in the following commands in cmd (Enter after each command) to push all the files to GitHub repository
   ```console
   git init
   git checkout -b directory_name_pages
   git add .
   git commit -m "initial commit#
   git remote add origin https://github.com/GitAccount/directory_name.git
   git push origin gh pages
   ```
   Go to the repository settings to find the website that you just created

   ![GitHub Push](https://raw.githubusercontent.com/AhirGit/Jekyll_Portfolio/comp3040A2_pages/GitHub%20Push.gif)

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
