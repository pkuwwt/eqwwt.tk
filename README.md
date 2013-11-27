eqwwt.tk
========

Host a website on github.

Step 1.
=======
Register a domain name. [[io.tk]] website provide free domain name.

Suppose you have registered a domain name `yourdomain.tk`


Step 2. 
=======
Create a repository in github, named as `REPO`. Pages in this repository are usually  **project pages**. See [[https://help.github.com/articles/user-organization-and-project-pages|user-organization-and-project-pages]]. If you use `username/username.github.io` as your repository name, this is a **user/organization** one, and one user can have the only one repository for hosting.

In `REPO` repository, create a `CNAME` file in `gh-pages` branches. Because this is a project one, other than **usr/organization**. In **usr/organization** case, you just use the `master` branch.

In `CNAME` file, input a single domain name, `yourdomain.tk`.

Step 3.
=======
Revise the DNS of the domain.
  * A Record: 
  * hostname: `yourdomain.tk`
  * IP:        `204.232.175.78`

Step 4.
=======
Wait for 10 minutes, you can access your website by `yourdomain.tk`. If you have a `index.html` file in the `gh-pages` branch of `REPO` repository, it's content will be displayed in browser by default.

Note:
=======
The tutorial above only setup a domain on project pages. If you want to setup subdomain like `subdomain.yourdomain.tk`, you should use **user pages**, and the IP will be like `username.github.io` other than `204.232.175.78`. And the IP will be auto-adjusted.

