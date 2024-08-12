<h1>Final Report for CSPB 3112: Learn to Build and Deploy a Microservices Web App</h1>

<p>During the semester, my primary goal was to learn new technologies that are being used extensively by companies today to build modern, microservices applications.
My research determined that the core technologies used for such a task are containers (commonly Docker containers) and Kubernetes to orchestrate the deployment of the
containers.  One can deploy Kubernetes from scratch wtihin their own data center or leverage a fully managed Kubernetes instance by one of the public cloud providers.
 For this project, I chose to leverage a fully managed Kubernetes instance in AWS known as AWS Elastic Kubernetes Instance or EKS.  To focus on learning these new technologies,
I leveraged a programming language and WSGI server that I was already familiar:  Python and Flask.  The following are the learning goals I had for the semester and my attainment of 
those goals.</p>

<h2>Goal 1 – Complete CloudAcademy Course: Introduction to Kubernetes</h2>

<p><b>STATUS:  ACHIEVED</b></p><br>

<p>I completed the Introduction to Kubernetes course on CloudAcademy and achieved a score of 100% on the final exam. I learned that Kubernetes is ideal for managing
microservices because it can orchestrate the deployment, scaling, and management of each microservice individually.  Labs allowed me to gain experience with each of the
core components of Kubernetes:  Cluster, Node, Pod, Service, Deployment, ConfigMap, and Secret.</p>

<h2>Goal 2 - Complete CloudAcademy Course: Docker in Depth</h2>

<p><b>STATUS:  ACHIEVED</b></p><br>

<p>I completed the Docker in Depth course on CloudAcademy and achieved a score of 92% on the final exam.  I learned that Docker is a container technology that is
widely used today and ideal for creating containers that would comprise my microservices web application.  Labs and training videos allowed me to learn about
Linux isolation and container basics, Docker container components, Docker networking and storage, and creating Docker images using Dockerfiles.</p>

<h2>Goal 3 – Complete CloudAcademy Course: Python based Microservices – Go from Zero to Hero</h2>

<p><b>STATUS:  ACHIEVED</b></p><br>

<p>I completed the Python-based Microservices course on CloudAcademy and achieved a score of 95% on the final exam.  I learned the fundamentals of a microservices architecture and
specifically how to leverage Flask to build small microservices that can be accessed via an application programming interface or API.  During the course, I completed several exercises that re-enforced the video-based learning.  Topics covered included container fundamentals, Introduction to Docker, Getting Started with Docker on Linux in AWS, Managing Applications with Docker Compose, Using Docker Compose and DockerFile to Build and Run Containers, and Building a Basic Web Application Using Python, Docker, and Flask. </p>

<h2>Goal 4 - Build and deploy a Python-based microservices web app using Docker containers and Kubernetes</h2>

<p><b>STATUS:  ACHIEVED</b></p><br>

<p>Over the course of the semester, I built a microservices web app called <a href="https://github.com/TrullJ/securitychkr">securitychkr</a>.  The web app allows a user to check whether a URL or email is malicious.  Additionally, a user can check the security status of a website's TLS/SSL certificate.  The idea behind the application is to provide one, convenient location for a user to determine whether or not emails and websites are trustworthy.  The website is comprised of four microservices deployed in the same number of containers.  The containers/microservices include the frontend container, urlvalidator container, emailvalidator container, and finally the sslvalicator container.  The worker containers leverage the VirusTotal, emailrep.io, and Qualys SSL Labs public services.  The frontend container presents a simple input field to the end user and then depending on input directs to one of the worker containers to perform the analysis and ultimately return the results to the frontend for display back to the user.  To learn modern methods of deploying and managing containers, I deployed the web app using AWS EKS. </p>

<h2>Reflections</h2>

<p>I found that the hands-on project and dedicated study time were a great way to get a solid understanding of containers, Docker, Kubernetes, and microservices architectures. The CloudAcademy courses were professionally done and covered the key components and use cases for the different technologies I wanted to gain experience.  One thing I would have changed in my approach is to build in more time reading the official documentation for each of the different technologies.  I referenced the official docs while building and deploying the web app and could have saved myself some rework by spending more time with the documentation and guides.  This was especially true for AWS EKS as I was required to re-write some of the code to ensure that the containers communicated properly with each other. The project also gave me an appreciation for the need to work together across teams to build and deploy a true production-grade application, and I learned a little more about the role of site reliability and devops engineers who are ultimately responsible for deploying and managing containers and ensuring the proper architecture exits to scale up an app and ensure proper security.  I am comfortable concluding that achieved my objectives set out at the beginning of the project and now have working knowledge a core set of modern technologies that will help me in my career.</p>

