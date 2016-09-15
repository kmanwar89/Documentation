### Quick guide on how to get Bootstrap up and running on GitHub pages with custom domain name

For my setup, I had my domain name of "kadaranwar.com" hosted on NameCheap

I consulted their great [guide](https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages) for step by step instructions on exactly how to link GitHub pages to the proper DNS entries.  In this case, I had to delete the A Name @ and www entries that used to lead to my VPS (hosted on DigitalOcean). Set the TTL to 1 for quick results.

Following the guides on GitHub, I created a repository named <GitHubusername>.github.io. The repo should have a file called CNAME with the only contents being the domain name I want to redirect to -- in this case, kadaranwar.com

Within this repo, I created an index.html file just for a quick test.  Using GitKraken, I committed/pushed the changes, and voila.

Now that the base page had been set up, I found a really nice one-page bootstrap template with [parallax scrolling](https://www.script-tutorials.com/bootstrap-one-page-template-with-parallax-effect/), but sadly they required me to "share" the page on Social Media in order to download all their files.  Thanks, but no thanks.  The code is on the page there and they provide a quick way to copy/paste, so I made my own file.

First, I downloaded [Bootstrap](https://github.com/twbs/bootstrap/releases/download/v3.3.7/bootstrap-3.3.7-dist.zip). Instead of extracting the contents of the .zip, I just drag/dropped the folders I needed into my kmanwar89.github.io repo folder on my local machine. This created three folders: css, fonts and js.

Next, I modified my index.html file to include all the source code from the template website before.

I created a separate style.css file in the css folder and pasted the code from the website, as well.

I pushed my changes, but the page wouldn't load because it didn't have the proper jQuery.min.js file. I found the file I needed on [this page](https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js) at the bottom of the Bootstrap landing page.  I copied/pasted the contents to a .js file of the same name.

Back in my template, I changed the jQuery version to match the one I just created.

Pushed my changes and everything works.

I chose to share the stupid website on my Google+ (which I subsequently deleted) in order to get access to the image files, though I could have manually scraped them from the page.

To get the Google Maps functionality working, I had to get an [API key](Documentation/API)

## Google Maps API Key
AIzaSyBs7I0vYf1-pg_oMHI6G4E-ppI9Xp-kvgg

content_copy


## Subdomains
So I can even do subdomains on GitHub pages.  It's as simple as creating a folder, adding an 'index.html' file to it, and pushing the changes from within GitKraken, as the drag/drop feature of GitHub doesn't support folders :(
