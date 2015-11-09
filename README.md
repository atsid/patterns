# patterns
ATS Patterns is here to help document how ATS writes proposals, sends reports, formats resumes, basically any and all office publications we want to prepare for client viewing.

We want everyone at ATS to contribute to the discussion about how we communicate business ideas! I'm borrowing heavily from the Engineer Guides, so Thank You to Travis, Evan et all for writing this out once already.

    Please fork the repo or create a branch, make changes, and submit a pull request to get your ideas reviewed by other developers.

This is a Bootstrap site, so it is both readable and editable using Markdown, and is deployable straight to GitHub Pages.

Once you've made all the edits you'd like, push your branch and submit a pull request. Once your pull request has been reviewed and discussed by the team, you should get a :shipit: or two indicating that it's ready to go. At that point, merge the branch into master, and the Travis build will automatically re-deploy the site to gh-pages.

The 'patterns' are individual pages that describe some aspect of how we deliver software and services to our customers. 

If you want to edit an existing page, simply work on it in your favorite editor. If you want to add a new guide page, add a new *.md file to the project root, and then insert the yaml header material. You can use one of the other pages as a template, but at a minimum you'll need the title, description, and permalink fields.
Blog Posts

We use Vagrant to streamline the installation of Jekyll so you can run the site locally to make sure any changes will look ok when deployed.

    vagrant up
    vagrant ssh
    cd /vagrant
    Start jekyll: jekyll serve
    View the site on your host machine: http://localhost:4000/guides

Deployment

Deployment uses a gulp task to push to gh-pages, where it can be viewed at http://labs.atsid.com/guides/.

    Get dev dependencies: npm install
    Install gulp if you don't have it: npm install -g gulp
    gulp deploy

Note again that this process happens automatically by Travis whenever commits are made to master.
