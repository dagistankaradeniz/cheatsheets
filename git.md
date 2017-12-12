# git - github cheat sheet
All explanations are OS independent. But if you are using Windows please setup and use [git](https://git-scm.com/downloads) to have **gitbash** that will add linux terminal environment to your operating system.

My personal choice is **Ubuntu 16.04 LTS**. Commands will be run on that OS.

## Install git
Add latest git PPA repository
```shell
$ sudo add-apt-repository ppa:git-core/ppa
```
Update your Ubuntu
```shell
$ sudo apt update
```
install git
```shell
$ sudo apt install git
```

Check git version
```shell
$ sudo git --version
```

For other OS please [click here](https://git-scm.com/download/linux)...

## Connect your local folder to your github account

Navigate inside your folder on terminal and type commands consequently
```shell
$ sudo git init
$ sudo git add .
$ sudo git commit -m "First Commit"
```
> The commands above are; create a .git folder, move all files and folders (. means everything) to staging area, and commit everything with a message.

Then connect to your github account (just copy your repository url and add to end of command below)
```shell
$ sudo git remote add origin <your_github_repository_url>
```
> You will be asked for your github **username** and **password**. Please enter correctly.

Then push your committed file and folders to github repository as master branch
```shell
$ sudo git push -u origin master
```

> **Note:**
> If you want to disconnect from your github account after you moved your works, please run
> ```shell
> $ sudo git remote remove origin
> ```

> **Note:**
> If you made mistake (or want to replace with new one) in remote URL and want to re-add new URL, please run
> ```shell
> $ sudo git remote set-url origin <your_NEW_github_repository_url>
> ```
