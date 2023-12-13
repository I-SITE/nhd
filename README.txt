This is a Wordpress repo for installation without composer package manager.

This repo assumes use of Astra theme, which is provided.

Provided plugins: 
  - astra-add-on to support Astra Pro license
  - astra-import-export to import and export theme config. 
  - go-live-update-urls to fix urls when changing from temmporary to live domains.
  - Siteground hosting helper plugins:
    -- Security optimizer
    -- Speed optimiser to manage Siteground caching

Recommended procedure to use:
  - Fork the repo to your own github account
  - Install the code on your host of choice, e.g. Siteground in the public_html directory
    -- Best practices is to use git version control to install, but you can download the files from github and upload to the host
  - Copy wp-config-sample.php as wp-config.php and update with database connection details
  - Use https://api.wordpress.org/secret-key/1.1/salt/ to generate salts to update wp-config.php
  - Set up wordpress in your web browser
  - update wordpress and plugins to latest versions
  - Enable the astra theme and at minimum the astra-import-export plugins
  - Import the astra configuration from the /astraconf directory to style the site like NHDPhilly.org
  - If theme changes are needed, some changes are available to the free version of astra. 
  - More comprehensive themeing can be accomplished by purchasing the Astra pro license and enabling the Astra add-on plugin
  - export and save astra config in /astraconf directory to preserve. 
  - committing changes to your github repo is recommended, as well as setting up backups on your host
