# Resume Host

## Purpose

**(Windows Only)**  
Step-by-step procedure of hosting a portfolio online using Jekyll Static Generator so that multiple  
employers can easily check through and the resume can be updated anytime

![DEMO](https://raw.githubusercontent.com/AhirGit/Jekyll_Portfolio/comp3040A2_pages/Resume%20Demo.gif)

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

    According to Etter, "GitHub Flavored  
    Markdown is a popular and fine choice for simple webbased help systems."  
    Therefore, using a markdown editor is our best option to create the resume  

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

3. Install gem package manager and Jekyll  
    Etter suggests that Jekyll is the most popular static site generator.  
    It can be used to create a beautiful functional documentation.  
    Hence, we use Jekyll to host a functional resume  

    Use the following commands in cmd

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

## Built With

* [VsCode](https://code.visualstudio.com/) - MarkDown Editor
* [Jekyll Site Generator](https://jekyllrb.com/) - Site Generator host

## More Resources

* **Andrew Etter** [Modern Technical Writing An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
* **Traversy Media** [Markdown Tutorial](https://www.youtube.com/watch?v=HUBNt18RFbo)
* **ScreentoGif** [Gif Recorder](https://www.screentogif.com/)

## Authors and Acknowledgements

* **Md Ahiduzzaman Ahir** - *Complete Work* - [AhirGit](https://github.com/AhirGit)
* **Billie Thompson** - *Template Inspiration* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## FAQS

1. A question about the overall process, such as "Why is Markdown better than a word
processor?"
    Becasue it is more functional and dynamic than word  

2. A question about the practical details, such as "Why is my resume not showing up?"
    Steps were not followed and tutorials were not watched properly

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details