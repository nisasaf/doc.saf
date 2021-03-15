# doc.saf = documentation by saf

Literally it's my personal documentation based on my experiences during learn about programming etc. But, it might be helpful to everyone. Anyway it would be contain random docs.

<h2>How to upload your project to Github repository</h2>
*Make sure that your project has been put together in one folder and you had installed Git in your computer.
And i recommend you to login first to Github account before push your project. Don't forget to creat new repository for your project.

1. Right click to your selected project folder.
2. Select Git Bash here.
3. Type these commands gradually:
4. jk
<ul>
  <li>git init</li>
  <li>git add *</li>
  <li>git commit -m "<i>commit</i>"</li>
  <li>git remote add origin https ://github.com/<i>yourUsername</i>/<i>yourRepository</i>.git</li>
  <li>git push origin master</li>
</ul>

*note: the italic words above means you could change it.

<h2>Set up Laravel project after cloned from Github</h2>
There are two ways to get started. It depends on your current condition.

<h3>If you already close your terminal after cloning the project, follow this way</h3>
1. Open your cloned local project.< 2. Make sure you've created the database for your cloned project. If not, please create it first.
3. Back to your cloned local project, copy an <b><i>.env.example</i></b> file and paste at the same path. 
4. Rename the file as <b><i>.env</i></b>
5. Then, right click wherever and choose GitBash here.
6. Type <b>composer install</b> click and enter to install the vendor folder.
7. After the installation process is complete, type <b>php artisan key:generate</b> and click enter.
8. Type <b>php artisan migrate</b> to make a migration.
9. Then, type <b>php artisan db:seed</b>.
10. Done. Now you can run your cloned project by type <b>php artisan serve</b> in terminal.

<h3>If you just cloned and not close your terminal, follow this way</h3>
1. Type <b>composer install</b> click and enter to install the vendor folder.
2. After the installation process is complete, type <b>php artisan key:generate</b> and click enter.
3. Type <b>php artisan migrate</b> to make a migration.
4. Then, type <b>php artisan db:seed</b>.
5. Done. Now you can run your cloned project by type <b>php artisan serve</b> in terminal.

<b>FINISH</b>
  
(see you in another update here.)
