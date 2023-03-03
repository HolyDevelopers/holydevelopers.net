Here you find the code behind https://www.holydevelopers.net. The website is running with [Drupal][Drupal.org] and managed with [composer][Drupal with composer].

It is using the coming Drupal default theme [Olivero][Olivero]. Currently it is a fairly simple setup with no customizations but just some modules installed.

Automatic deployment is set up using our [php-webhook-handler][php-webhook-handler] (more explanations: [Deploying to a web server using GitHub webhooks][deploying]). The test branch is deploying to a test system.

## Requirements
* PHP (8.1 recommended), MySQL, Apache, Composer (version 2 recommended)

## Installation
* clone the repository
* `composer install`
* setting up MySQL database:
  * `CREATE DATABASE holydevelopers;`
  * `CREATE USER holydevelopers@localhost IDENTIFIED BY 'TODO YOUR PASSWORD'`
  * `GRANT ALL PRIVILEGES ON holydevelopers.* to holydevelopers@localhost;`
  * `FLUSH PRIVILEGES;`
* Make sure the directory `sites/default/files` is writable for Apache
* `drush site:install`

## Next steps
* provide database dump
* setup [Gitpod][Gitpod] for easy development and contribution
* let users subscribe to topics and get automatic notifications on new posts containing a tag they're interested (using DANSE?)

## License
Jesus says in Matthew 10:8, “Freely you have received; freely give.”
We follow His example and believe His principles are well expressed in the developer world through free and open-source software.
That's why we want you to have the ["four freedoms"](https://fsfe.org/freesoftware/) to freely use, study, share and improve this software.
We only require you to release any derived work under the same conditions (you're not allowed to take this code, build upon it and make the result proprietary):

[GNU General Public License v2.0 or later](LICENSE.txt)

This is the same license used for all Drupal code.

## Contributing

By contributing you release your contributed code under the licensing terms explained above. Thank you!

[Drupal.org]: https://www.drupal.org
[Drupal with composer]: https://www.drupal.org/docs/develop/using-composer
[Olivero]: https://www.drupal.org/docs/core-modules-and-themes/core-themes/olivero
[php-webhook-handler]: https://github.com/HolyDevelopers/php-webhook-handler
[deploying]: https://www.holydevelopers.net/deploying-to-a-web-server-using-github-webhooks
[DANSE]: https://www.drupal.org/project/danse
[Gitpod]: https://www.gitpod.io/
