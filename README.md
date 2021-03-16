# doc.saf = documentation by saf

Literally it's my personal documentation based on my experiences during learn about programming etc. But, it might be helpful to everyone. Anyway it would be contain random docs.

<h2>How to upload your project to Github repository</h2>
*Make sure that your project has been put together in one folder and you had installed Git in your computer.
And i recommend you to login first to Github account before push your project. Don't forget to create new repository for your project.

1. Right click to your selected project folder.
2. Select Git Bash here.
3. Type these commands gradually:
> <ul>
    <li>git init</li>
    <li>git add *</li>
    <li>git commit -m "<i>commit</i>"</li>
    <li>git remote add origin https ://github.com/<i>yourUsername</i>/<i>yourRepository</i>.git</li>
    <li>git push origin master</li
  </ul>  
    
*note: the italic words above means you could change it.

<h2>Set up Laravel project after cloned from Github</h2>
*There are two ways to get started. It depends on the conditions of your cloning project.
  
*If you already close your terminal after cloning the project, follow this way.
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

*If you just cloned and not close your terminal, follow this way.
1. Type <b>composer install</b> click and enter to install the vendor folder.
2. After the installation process is complete, type <b>php artisan key:generate</b> and click enter.
3. Type <b>php artisan migrate</b> to make a migration.
4. Then, type <b>php artisan db:seed</b>.
5. Done. Now you can run your cloned project by type <b>php artisan serve</b> in terminal.

<h2>Set upstream branch in Github</h2>
*Make sure you've forked the project to your GitHub account and clone it to your local repo.

1. First, clone the forked project by type <b>php artisan clone</b> <i>https://,span></span>github.com/<b>your_username</b>/<b>file_name</b>.git</i>
3. Then, open your cloned local project that you've forked.
4. Right click wherever and select GitBash here.
5. Type <b>git remote -v</b> to see the current configured remote repository of your fork. The result should be:  
    
   > <b>origin https://<span></span>github.com/<i>your_username</i>/<i>your_file</i>.git (fetch)  
   > <b>origin https://<span></span>github.com/<i>your_username</i>/<i>your_file</i>.git (push)
7. 

<b>FINISH</b>
  
(see you in another update here.)
