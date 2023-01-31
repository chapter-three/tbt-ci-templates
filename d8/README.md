# Drupal 8

## Note

Given that Drupal 8 is EOL since November 2021, this is NOT MAINTAINED anymore.

-----

This folder contains different files and configurations for Drupal 8 sites.

For any CI provider, you should copy the .ci folder to your project root and the corresponding folder under the providers folder also to your project root. Then, follow the instructions in the right section below.

## CircleCI

If you need to enable CircleCI for an existing project, after copying files you should add the following environment variables to CircleCI configuration:

- ADMIN_EMAIL
- ADMIN_PASSWORD
- ADMIN_USERNAME
- TERMINUS_TOKEN
- TERMINUS_SITE
- GITHUB_TOKEN
- GIT_EMAIL
- TEST_SITE_NAME

Also, a ssh private key should be added to the project configuration and the corresponding public key should be added to a Pantheon account with enough permissions over the site.

## Gitlab CI

If you need to enable GitlabCI for an existing project, after copying files you should add the following environment variables to GitlabCI configuration:

- ADMIN_EMAIL
- ADMIN_PASSWORD
- ADMIN_USERNAME
- TERMINUS_TOKEN
- TERMINUS_SITE
- GITLAB_TOKEN
- GIT_EMAIL
- TEST_SITE_NAME
- SSH_PRIVATE_KEY
- TERMINUS_BUILD_TOOLS_PROVIDER_GIT_GITLAB_URL

The TERMINUS_BUILD_TOOLS_PROVIDER_GIT_GITLAB_URL value will be "gitlab.com" or your gitlab instance domain.

## Bitbucket Pipelines

If you need to enable Bitbucket Pipelines for an existing project, after copying files you should add the following environment variables to Bitbucket Pipelines configuration:

- ADMIN_EMAIL
- ADMIN_PASSWORD
- ADMIN_USERNAME
- TERMINUS_TOKEN
- TERMINUS_SITE
- BITBUCKET_USER
- BITBUCKET_PASS
- BITBUCKET_AUTH
- GIT_EMAIL
- TEST_SITE_NAME
- COMPOSER_AUTH
- SSH_PRIVATE_KEY

## Github Actions

If you need to enable Github Actions for an existing project, after copying files you should add the following secrets to Github Actions configuration:

- ADMIN_EMAIL
- ADMIN_PASSWORD
- ADMIN_USERNAME
- TERMINUS_TOKEN
- TERMINUS_SITE
- SSH_PRIVATE_KEY
- GH_TOKEN
