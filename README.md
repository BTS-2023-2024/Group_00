## Developers
| Name        |   Role |     Github    | Email       |
| ----------- | --------- | --------- | --------------------------- |
| Marcel Jar  | Back-End Dev | marceljar | marcel.jar@senecacollege.ca |
| Tony Stark  | Front-End Dev |tonystark | tony.stark@senecacollege.ca |
| Bruce Banner  | Database Specialist | brucebanner | bruce.banner1@senecacollege.ca |

## Project Description
In this project, a website tailored for faculty members teaching CAPSTONE project courses is developed. This website will feature a few tools to aid faculty during the process of teaching these courses. The three most important tools are a timeslot picking tool, a group messaging tool, and a login system, which are presented in what follows:

### Timeslot Picking Tool
This tool will allow faculty members to create timeslots available for groups of students to pick their preferred meeting times. After the timeslots are created, students are able to log in and click on available timeslots. This tool should also send a message to all group members with details about the chosen timeslots. Note that the tool does not have an option to allow students to change their chosen option. This is done by design. The idea is to prevent students from picking a timeslot as a placeholder first, and then discussing timeslots with other team mates later.

### Group Messaging Tool
This tool will allow the faculty to quickly visualize all groups and its members. Moreover, this toll should allow faculty to quickly craft an email message to specific groups.

### Login System
Both tools presented above require the website to have an authentication system in which users can take two different roles (faculty or student), each role with specific capabilities. Due to the fact that users are only allowed into the system as per faculty's invitation, no authentication APIs, such as [Facebook](https://developers.facebook.com/docs/facebook-login/), or [Google](https://developers.google.com/identity/sign-in/web/sign-in), are implemented. Moreover, since the website only stores students' emails and their selected timeslots, no concerted effort has been made to secure the information stored in the system.

## Tech Stack

### Back-End

The website is served by an [Apache 2.0](https://httpd.apache.org/) server, running on an Ubuntu 18.04 OS hosted by [Digital Ocean](https://www.digitalocean.com/). It uses a [Django](https://www.djangoproject.com/) framework. This framework implements a model-template-view pattern that links together a number of Python scripts and a SQLite database to render all pages transmitted to the end-user via HTTP. 

### Front-End

In its Front-End, the website uses [Bootstrap 3.3](https://getbootstrap.com/docs/3.3/) to create a responsive experience. Moreover, the [JQuery](https://jquery.com/) library,  which is required by this version of Bootstrap, is used to simplify the coding of AJAX calls. No other JavaScript libraries are used.

### Developing Tools

This website was developed using [Visual Studio Code](https://code.visualstudio.com/) with a Python and Remote-SSH extensions. [Postman](https://www.postman.com/) was used to test HTTP requests in order to decouple back-end and front-end tasks.


