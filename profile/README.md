<img src="../../../application-store/img/silicolab_logo.png" align="right"
     alt="Size Limit logo by Anton Lovchikov" width="60" height="60">

# Welcome to the BIBBOX Repository

The BIBBOX allows researchers to publish their data and the associated data management software (Apps) in a FAIR manner, through the incorporation of a FAIR Data Point into the Apps. 
The architecture of the BIBBOX is modular and flexible, allowing researchers to add a FAIR Data Point to existing open-source software solutions and to publish these in the App Store. The main components of the BIBBOX architecture (Frontend/Backend) are stored on the [**sys-bibbox**](https://github.com/bibbox/sys-bibbox) repository.


## How to contribute to the BIBBOX?

You can create a BIBBOX App! 

If you have an open-source software solution, you can easily transform it into a BIBBOX App, following the tutorial at [http://bibbox.bbmri-eric.eu/create-a-bibbox-app/](http://bibbox.bbmri-eric.eu/create-a-bibbox-app/).


## How to create a BIBBOX App?

Each BIBBOX App must be published in a repository named **app-nameofapp**. The repository [**app-template**](https://github.com/bibbox/app-template) aims to guide you when creating an App. 

### The most important steps to generate a BIBBOX App are:

The Base Docker is a container created from a Docker Image of the existing software tool. The officially published Docker Image of the software can be used. If none is available, a Dockerfile of the Docker Image should be stored in a BIBBOX GitHub repository named **img-nameofdocker** and the Docker Image published in the [BIBBOX Docker Hub](https://hub.docker.com/u/bibbox/). If necessary,  additional Docker Containers of the App, such as databases, can be integrated with the Docker Image of the Base Docker.

In order to register an App in the BIBBOX, the files [applications.json](https://github.com/bibbox/application-store/blob/master/applications.json)  and [bibbox.json](https://github.com/bibbox/application-store/blob/master/bibbox.json) of the [application-store](https://github.com/bibbox/application-store) repository have to be extended.




