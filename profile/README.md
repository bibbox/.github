# Welcome to the BIBBOX Repository

The BIBBOX allows researchers to publish their data and the associated data management software (Apps) in a FAIR manner, through the incorporation of a FAIR Data Point into the Apps. 
The BIBBOX supports the creation and management of FAIR Data Points. The architecture of the BIBBOX is modular and flexible, allowing researchers to add a FAIR Data Point to existing open-source software solutions and to publish these in an App Store. The main components of the BIBBOX architecture (Frontend/Backend) are stored on the [**sys-bibbox**](https://github.com/bibbox/sys-bibbox) repository.


## How to contribute to the BIBBOX?

You can create a BIBBOX App! 

If you have an open-source software solution, you can easily transform it into a BIBBOX App, following the tutorial at [http://bibbox.bbmri-eric.eu/create-a-bibbox-app/)](http://bibbox.bbmri-eric.eu/create-a-bibbox-app/).


## How to create a BIBBOX App?

Each BIBBOX App must be published in the BIBBOX GitHub repository [32], by creating a repository named **app-nameofapp**. The repository [**app-template**](https://github.com/bibbox/app-template) aims to guide you when creating an App. 

### The most important steps to generate a BIBBOX App are:

The Base Docker is a container created from a Docker Image of the existing software tool. The officially published Docker Image of the software can be used. If none is available, a Dockerfile of the Docker Image should be stored in a BIBBOX GitHub repository named **img-nameofdocker** and the Docker Image published in the [BIBBOX Docker Hub](https://hub.docker.com/u/bibbox/).



Additional Docker Containers of the App, such as databases, can be integrated with the Docker Image of the Base Docker, resulting in a docker-compose file, which should be published in the **app-nameofapp** repository. 
Docker Images of the additional Docker Containers can, if necessary, be published in the BIBBOX GitHub repository and in the BIBBOX Docker Hub.

In order to register an App in the BIBBOX, two configuration files of repository application-store have to be extended:  [applications.json](https://github.com/bibbox/application-store/blob/master/applications.json)  and [bibbox.json](https://github.com/bibbox/application-store/blob/master/bibbox.json).

The file **applications.json** maps the  App repository to a human-readable name of the App. The file **bibbox.json** groups the Apps into specific categories, according to their functionality. 
Once the App is published in the BIBBOX GitHub repository, it becomes available for installation at the App Store of the BIBBOX Portal. Once a user installs an App, its installation will appear on "App Instances". Users can browse all the Apps available in the "App Store" and install them.  In the "App Instances", users can access all the current installation instances of the Apps.




