# deployed-my-website-as-a-container

<p>## Here is how I containerized my website

As a prerequisite, ensure that you have docker installed locally on your machine. [Install Docker Engine](https://docs.docker.com/engine/install/)

The code for my website is hosted on [GitHub](https://github.com/paschalogu/personal-website).  To follow along, fork and clone this repository and change directory into it by running the commands below:</p>

<p style="background-color: grey">
git clone <span>https://github.com/paschalogu/personal-website.git</span><br>
cd personal-website</p>

<p><u>## Step 1: Build the Docker image</u>

- Add a Dockerfile

I created a new file named **Dockerfile** by running the command `touch Dockerfile` in the root of my website directory and added these lines of code below inside the Dockerfile:</p>
<p>FROM nginx:alpine <br>

COPY . /usr/share/nginx/html <br>

EXPOSE 80</p>
- Build Image

Then I built the image by running the line of code below: <br>
docker build -t personal-website:v1 .</b>
</p>
<p>## Step 2: Push to Docker Registry

I logged in to [Docker Hub Container Image Library](https://hub.docker.com/) and created a new repository.  I named it `personal-website` and gave it a short description (description is optional).</p>



