# BIBBOX 

This is the BIBBOX repository.
The main components of the BIBBOX (Frintend/Backend) are stored on the sys-bibbox repository.

## How to contribute to the BIBBOX?




## How to create a BIBBOX App?

Starting with an existing open-source software solution that handles data, one can easily transform it into a BIBBOX App, following the tutorial at {https://bibbox.readthedocs.io/en/latest/}[https://bibbox.readthedocs.io/en/latest/].

Each BIBBOX App must be published in the BIBBOX GitHub repository [32], by creating a repository named app-nameofapp. The repository app-template [33] aims to guide users when creating an App. 


The most important steps to generate a BIBBOX App are:
The Base Docker is a container created from a Docker Image of the existing software tool. The officially published Docker Image of the software can be used. If none is available, a Dockerfile of the Docker Image should be stored in a BIBBOX GitHub repository named img-nameofdocker and the Docker Image published in the BIBBOX Docker Hub [34].
Additional Docker Containers of the App, such as databases, can be integrated with the Docker Image of the Base Docker, resulting in a docker-compose file, which should be published in the app-nameofapp repository. As depicted in Figure 7, the Docker Images of the additional Docker Containers can, if necessary, be published in the BIBBOX GitHub repository and in the BIBBOX Docker Hub.
The FAIR Data Point is recommended for Apps that handle data, in order to make the data FAIR. For the extension of an App with a FAIR Data Point (FDP), the different components of the FDP are combined into a Docker Image and published in the BIBBOX Docker Hub. As many Apps do not internally support FDPs, the appropriate metadata of the App must be extracted and transformed by the middleware and then loaded into the FDP.
In order to register an App in the BIBBOX, two configuration files in the BIBBOX repository application-store have to be extended:  applications.json and bibbox.json. The file applications.json maps the  App repository to a human-readable name of the App. The file bibbox.json groups the Apps into specific categories, according to their functionality. Once the App is published in the BIBBOX GitHub repository, it becomes available for installation at the App Store of the BIBBOX Portal. Once a user installs an App, its installation will appear on "App Instances". As shown in Figure 8, users can browse all the Apps available in the "App Store" and install them.  In the "App Instances", users can access all the current installation instances of the Apps.



**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
