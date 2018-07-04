# busuu builds dashboard

This is a build status dashboard for busuu based on [Dashing]. Build information is read from [Jenkins JSON REST APIs] and displayed in micro-apps on a pretty dashboard.

# Requirements
Ruby is required to run this project (version 1.9+ but 2.2.1 recommended). First install [rvm]. Then use rvm to install ruby:
```sh
$ rvm install 2.2.1
```

# Running the dashboard
1. Install [Dashing] and [Bundler]:

    ```sh
    $ gem install dashing
    $ gem install bundler
    ```
2. Change directory to the root of this repo:

    ```sh
    $ cd builds-dashboard
    ```
3. Install required gems using Bundler:

    ```sh
    $ bundle
    ```
4. Start the server:

    ```sh
    $ dashing start
    ```
5. View your dashboard in a web browser at <http://localhost:3030/builds>

[//]: #
[dashing]: <http://dashing.io/>
[Jenkins JSON REST APIs]: <https://wiki.jenkins-ci.org/display/JENKINS/Remote+access+API>
[Bundler]: <http://bundler.io/>
[rvm]: <https://rvm.io/>
