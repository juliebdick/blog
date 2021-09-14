# Introduction Post
<h2>Installing Ruby</h2>
When I ran ruby --version, I already had ruby 2.3.7, but I went ahead and installed ruby from the command line. I then needed to change the permissions in my machine and run brew doctor in order to run gem install bundler. Brew doctor gave interesting and useful outputs, so I'm glad I discovered that.

<h2>Installing Jekyll</h2>
When installing Jekyll, I created a Gemfile.txt. But when I ran bundle install, I got an error that the machine could not locate my Gemfile. I was unsure of what the problem could be. After some <a href="https://forestry.io/docs/troubleshooting/could-not-locate-gemfile-or-bundle-directory/">research</a>, I learned you could create a Gemfile by running bundle init. It was then that I learned the file must be named "Gemfile" and not "Gemfile.txt."
I was missing a gem, so I had to run bundle install a second time and 30 missing gems were installed. Installing Ruby and Jekyll from the command line was user friendly and easy to follow. I'm pleased with using this method of installation.

<h2>Fixing the Default Blog</h2>
When editing the default Jekyll blog, I used a colon in my title. I received an email from GitHub that my page was unable to build because I had an error on line 16 of my _config.yml file, and there was a <a href="https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/troubleshooting-jekyll-build-errors-for-github-pages-sites#config-file-error">link</a> attached to the email with ways to troubleshoot my error. This was awesome. I learned you must quote any special characters (including colons) that you use in the _config.yml file.

<h2>Key Takeaways</h2>
<ul>
<li>The command line gives useful feedback.</li>
<li>Having a text editor like Atom is helpful.</li>
<li>The default Jekyll blog is thorough and seems simple to work with.</li>
</ul>
