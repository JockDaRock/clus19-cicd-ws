# clus19-cicd-ws

https://github.com/JockDaRock/clus19-cicd-ws

# Guide of commands and code for the workshop

* Login to sites with creds... User: `cicd-userX` (replace X with your number) Password: cisco

Drone `https://17c85ec1.ngrok.io`
Gogs `https://f7c68928.ngrok.io/`

* In Gogs we will import our code. Follow along on the screen.  You will use the below URL to import our codebase.

```bash
https://github.com/CiscoDevNet/cicd-idpw-sample-code
```

* Next we will activate our repo.  Follow along with the instructor to activate the repo and drone connection.

* Login to Fog Director with creds... User: `admin` Password: `admin_123`

```bash
https://4cb7b1c6.ngrok.io
```

* Start the docker container we will use to connect to our lab content

* Open a terminal window and run the following command.

```bash
docker run -it -p 127.0.0.1:8443:8443 ciscodevnet/vs-cicd-ws-code:latest --allow-http --no-auth
```

* In your browser, navigate to `http://127.0.0.1:8443`.

From here on out we will work in the web based code editor and terminal.

* In the VS Code site open a terminal window

* In the that terminal window, import our codebase with the following command.

```bash
git clone https://f7c68928.ngrok.io/cicd-user<#>/idpw-user<#>
```

* Now follow the instructor above to edit our CICD pipeline code and repository information for the pipeline build.

...
...
...
...
...

* On the terminal window change directories into our code repo folder

```
cd idpw-user<#>
```

* Use git to add our user name and e-mail

```
git config --global user.email cicd-user<#>@devnet.org

git config --global user.name cicd-user<#>
```

* Run the following commands to push up our code.

```
git add --all

git commit -m "CICD Let's GO!!!"

git push origin master
```

* Go back to then drone tab in your browser and view the build.

If you want to give it another try after this workshop... visit the online DevNet Learning Lab for CICD w/ IOx apps.

https://developer.cisco.com/learning/tracks/iot/cicd-iox/iox-app-building-cicd/step/1



