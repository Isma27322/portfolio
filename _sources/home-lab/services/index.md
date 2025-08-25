# What's Running on the Lab

I use Docker to run everything, which makes it fun and easy to spin up new services. 
Here's what I'm currently hosting:

---
### Jellyfin
<img src="../../_static/Jellyfin-logo.png" width="80" height="80" style="background-color: transparent;"/>
<!-- insert jellyfin logo -->

* **What it is:** Jellyfin is a community-driven, self-hostable media server system that lets you manage and stream your own media collection without subscriptions or external dependencies.
* **Why I run it:** I wanted to be able to have videos and music locally hosted.
* **Coolest thing I learned:** I learned how much Jellyfin relies on good file naming to pull in all the correct posters and
show information. \
I also found it really handy that it automatically saves my watch progress, making it easy to resume a movie or show later on any device.

---
### NGINX Proxy 
<img src="../../_static/nginx-logo.png" width="80" height="80" style="background-color: transparent;"/>

* **What it is:** NGINX is a high-performance, self-hostable built-in reverse proxy that intercepts client requests and forwards them to appropriate backend servers—enhancing load balancing, security, and scalability.
* **Why I run it:** It is handy to be able to only enter a domain with a subdomain and have it lead to that service with no extra ports on the domain.
* **Coolest thing I learned:** I think the coolest thing I learned is that this functionality is built right into NGINX. I also figured out how to use local-only domains (like jellyfin.dellinux.local) to point directly to a service's IP and port, like 192.168.40.22:8096. Another neat discovery was that by default, NGINX forwards any requests to the server's main IP address to the first service listed in the proxy configuration.

---
### NGINX Web Server
* **What it is:** NGINX is a high-performance, self-hostable HTTP web server designed for serving static and dynamic content with minimal resource usage, built on an event-driven, asynchronous architecture that ensures exceptional speed and scalability.
* **Why I run it:** It is handy to be able to easily run a web server without the hassle of seting it up yourself.
* **Coolest thing I learned:** I honestly didn't learn much with this one, as it worked out of the box!

---
### Home Assistant 
<img src="../../_static/homeassistant-logo.png" width="80" height="80" style="background-color: transparent;"/> <!-- Insert ha logo -->

* **What it is:** Home Assistant is an open-source, self-hostable smart-home automation platform that brings all your devices under local control with privacy and flexibility.
* **Why I run it:** I wanted an open source home automation application for my smart devices. I wanted local control and not haveing to rely on the cloud to control my devices.
* **Coolest thing I learned:** I learned that my current smart devices are not natively supported by home assistant. I discovered the HACS (Home assistant Community Store) that allowed me to control my normally cloud only devices from a local only connection. I also learned that it can support a lot of smart devices right out of the box with no extra configuring needed.

---
### n8n 
<img src="../../_static/n8n-logo.png" width="200" height="50" style="background-color: transparent;"/><!-- insert n8n logo -->

* **What it is:** n8n is a powerful, flexible automation workflow tool that uniquely serves as a self-hostable automation workflow tool, enabling technical teams to build complex, code-enabled automations or drag-and-drop workflows with full control over deployment.
* **Why I run it:** I run n8n because it is handy to have, and it can perform program-like automation that connects with almost any external app.
* **Coolest thing I learned:** Some of the coolest things I learned are the number of things that n8n can talk to: home assistant, discord, gmail, and so much more. It is able to do it without too much setup from the end user. \
I also like that it is so easy to understand what is happening while it is happening. \
You are also able to easily see where an error occurred.

---
### Docker 
<img src="../../_static/Docker-Logo.png" width="160" height="80" style="background-color: transparent;"/><!-- insert docker logo -->

* **What it is:** Docker is a flexible, self-hostable containerization platform that lets you deploy and run applications in lightweight, isolated containers across environments.
* **Why I run it:** You can run many containerized apps on one server. This is more efficient than them each being on their own dedicated server.
    * You can run an app without having to worry about it affecting the host system or other Docker apps.
    * You can run a lightweight virtual machine (VM) with an easy setup
    * You are able to run any application in a containerized format.
* **Coolest thing I learned:**
Some of the coolest things I learned is how Docker works. It's like a regular VM but without dedicated resources; it can use the host's resources with no dedicated guest resources. \
Another cool thing I learned with Docker is that, like a VM, you can run a different operating system (mostly Linux), even if it is different from the host operating system.