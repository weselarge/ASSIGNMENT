#QUESTION 1: APACHE WEBSITE
## Requirement:
* Dockerfile
* index html file

* Dockerfile: Create a file with the touch cmd and populate with the code below

FROM httpd:2.4

COPY index.html /usr/local/apache2/htdocs/[image](./apache1.png)

* index html file: Create an index.html file and populate with the code below in this [image](./apacheHTML.png)

Build the Dockerfile, then run the image specifying the port.

[output on web browser](./apache_website.png)




