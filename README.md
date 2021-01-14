# OAK Website

This repository contains the source for the OAK website hosted at awakeningkindness.org. It is a static site that uses [hugo](https://gohugo.io/) to generate HTML and CSS files from a set of .toml files.

To modify the website you should: open a pull request, get a review, and then merge the pull request (more info below). Each merge to master will be automatically deployed to awakeningkindness.org.

## Getting access

To make changes to the website:

1. Create a Github account if you do not already have one. If you have a personal Github account using your personal email address, it is fine to use that. There is no need to create a separate account using your CML email address.

2. Ask Kōshin to add you as a collaborator on the Github repository.

To troublshoot technical issues and tinker with the deployment infrastructure:

1. Create a Digital Ocean account

2. Ask Kōshin or Jōshin to add you to the OAK organization on Digital Ocean

## Making changes

Making small changes using the Github web interface:

1. Navigate to the [repository on Github](https://github.com/alexflint/awakeningkindness.org)

2. Navigate to the `content` directory

3. Click on one of the markdown files (`_index.md` is the home page)

4. Click the edit icon next to  in the top right

5. Make the appropriate change

6. At the bottom of the page select "Create a new branch for this commit and start a pull request."

7. Click "Propose changes"

8. Write a description of what you changed in the title box and a longer description of why in the main text section

9. Click "Create pull request"

10. Tell Kōshin that you have created a pull request and send him a link to your pull request

11. Make any requested changes

12. After the pull request has been approved, click "Merge"

13. Wait for 2 minutes and then check https://awakeningkindness.org/ for the live changes

Making larger changes using command-line git:

1. Install git

2. Clone the repository with `git clone git@github.com:alexflint/awakeningkindness.org.git`

3. Create a branch with `git checkout -b new-branch-name`

3. Make the edits locally

4. Commit changes with `git commit -m "message about what I changed`

5. Push changes with `git push -u`

6. Go to Github in your web browser and create a pull request for the branch

7. Follow the review and merge instructions from the section above

## Testing it locally

1. Install [hugo](https://gohugo.io/)

2. Clone the repository locally (see above)

3. Run `make serve`

4. Navigate to `http://localhost:1313/`

## Deployment

This website is hosted on the DigitalOcean App Platform as a static site. The deployment system is configured to watch for pushes to the master branch of the Github repository and deploy them to the production site.

## Domains

The domain awakeningkindness.org was purchased using Google Domains under koshin@cml.me for $12/yr billed to OAK. We have since purchased several related domains on this same account, such as awakenedkindness.org and awakenkindness.org.

## Troubleshooting

If changes fail to show up on the production website, try this:

1. Log into the DigitalOcean control panel (see "Getting Access" above)

2. Navigating to the "OAK" project

3. Navigate to "Apps"

4. Click on "awakwningkindness.org"

5. Click "Deployments" tab and check the status of the top deployment. If it says "Error" then click "Details" on the right.

To reproduce a production build locally:

1. In the DigitalOcean control panel for the "awakeningkindness.org" app, click on "Components" and make sure the "awakeningkindness.org" component is selected

2. Go down to "build" and copy the build command to your terminal

# TODO

* Set up www.awakeningkindness.org to redirect to awakeningkindness.org

  
