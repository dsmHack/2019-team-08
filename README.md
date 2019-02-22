# IRIS

Repo for the IRIS dsmHack team 2019

### How to build:

- Create env: `cp .env.example .env`

### How to run:

- Start: `docker-compose up`
- Stop: `docker-compose down`

### Documentation:

Start the application locally and navigate to `localhost:80`

### Gotchas and Tips:

- In my case, `"$(pwd)"` was `///c/Users/[Your Windows username here]/workspace/2018_team_1_api`. Full command looks like this: `docker run -it --rm --name my-maven-project -v ///c/path/to/the/repo/2018_team_1_api:/project maven:3.3-jdk-8 mvn -f project/ clean package`
- If you get this error message: `the input device is not a TTY.  If you are using mintty, try prefixing the command with 'winpty'` add `winpty` to the beginning of your command. Here's why: http://willi.am/blog/2016/08/08/docker-for-windows-interactive-sessions-in-mintty-git-bash/
- Add `-d` to `docker-compose up` to background. The process can be found by running `docker ps` and `docker stop [container id]`.```

