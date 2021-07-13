# better-abstracts-project
This is a Composer-based installer for the [Better Abstracts](https://www.drupal.org/sandbox/skounis/3218699) Drupal distribution.

# Installation
```
composer create-project betterevents/better-abstracts-project --stability dev MY_PROJECT
```
This will create a functioning Better Abstracts site and install all the project's dependencies. Continue with the installation like you would with any other Drupal site.
1. Create a database per [Drupal's documentation](https://www.drupal.org/docs/installing-drupal/step-3-create-a-database).
2. Open a web browser and visit `core/install.php`.
3. [Run the installer](https://www.drupal.org/docs/installing-drupal/step-5-run-the-installer).


## Docker Container
Request the project without installing depedencies
```
composer create-project betterevents/better-abstracts-project --stability dev --no-install my-abstracts
```

Start the container: 
`docker-compose up`

It's advised to not daemonize docker-compose so you can turn it off (CTRL+C) quickly when you're done working. However, if you'd like to daemonize it, you have to add the flag -d:
```
docker-compose up -d
```

Then Require depedencies:
```
docker-compose exec web composer install` 
```

Open a web browser and visit http://localhost:8080/web


# Usage
You are all set to put it into action! Next steps:

1. Populate Better Abstracts with sample content
2. Learn how to configure and use it.

Get started with our [quick start guide](https://docs.google.com/document/d/1OolrXm3ynUR_kwSOrBM8Yevh1eYSVD0uJ-wAONpOn8c/edit?usp=sharing) or read our [full documentation](https://docs.google.com/document/d/13CNN5PFDv54cfhCdnZT_F6epfnNxXIVkyMyhF_qeTAQ/edit?usp=sharing).
