# doc.saf = documentation by saf

Literally it's my personal documentation based on my experiences during learn about programming etc. But, it might be helpful to everyone. Anyway it would be contain random docs.

<h2>How to upload your project to Github repository</h2>
Make sure that your project has been put together in one folder and you had installed Git in your computer.
And i recommend you to login first to Github account before push your project. Don't forget to create new repository for your project.

1. Right click to your selected project folder.
2. Select Git Bash here.
3. Type these commands gradually:
```
    git init
    git add *
    git commit -m "commit"
    git remote add origin https://github.com/yourUsername/yourRepository.git
    git push origin master
````  
    
*note: that <b>commit</b> word could changed with your own commit message.

<h2>Set up Laravel project after cloned from Github</h2>
There are two ways to get started. It depends on the conditions of your cloning project.
  
If you already close your terminal after cloning the project, follow this way.
1. Open your cloned local project.
2. Make sure you've created the database for your cloned project. If not, please create it first.
3. Back to your cloned local project, copy an <b><i>.env.example</i></b> file and paste at the same path. 
4. Rename the file as <b><i>.env</i></b>
5. Then, right click wherever and select GitBash here.
6. Type <b>composer install</b> and enter to install the vendor folder.
7. After the installation process is complete, type <b>php artisan key:generate</b> and click enter.
8. Type <b>php artisan migrate</b> to make a migration.
9. Then, type <b>php artisan db:seed</b>.
10. Done. Now you can run your cloned project by type <b>php artisan serve</b> in terminal.

If you just cloned and not close your terminal, follow this way.
1. Type <b>composer install</b> click and enter to install the vendor folder.
2. After the installation process is complete, type <b>php artisan key:generate</b> and click enter.
3. Type <b>php artisan migrate</b> to make a migration.
4. Then, type <b>php artisan db:seed</b>.
5. Done. Now you can run your cloned project by type <b>php artisan serve</b> in terminal.

<h2>Use Multiple Github Account in One Device</h2>
I followed this way <i>(click: https://dev.to/jogendra/how-to-use-multiple-github-accounts-on-single-machine-2me9)</i> to set multiple github account. Just jump up to the <b>Use SSH</b> part to follow the steps. In <b>Step 2</b>, you'll see the command like:


```
    pbcopy < ~/.ssh/id_rsa_work.pub
```

If you are a Windows user, you can replace ```pbcopy``` to ```clip``` to copy your work account SSh key to machine clipboard.
You can ignore <b>Step 3</b> and just continue to <b>Step 4</b>.
<i>note: seriously, if you're a very very very beginner just like me, don't ever try Step 3, cuz i've did it and end up spend some hours to solve the issue. hehehe</i>

Alright, next. If you test the rules and still can't, try to re-add remote URL. 

```
    git remote remove <remote-name>
    git remote add origin git@<host>:<username>/<repo-name>.git
    ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts
```

And then, try to push again. 

<b>FINISH</b>
  
(see you in another update here.)
