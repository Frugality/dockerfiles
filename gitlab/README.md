# NOTE (deprecated)
There is no need to use this hack anymore. Literally the next day, after making this, the original project made the needed variables available though config.

I'l keep this project around just because it’s a nice hack and it will work on other projects as well. But for this exact project, read their documentation about how to enable Google authentication without hacks :)

# Old README

The (currently) only purpose of this container is to support Google oauth2 for the gitlab container sameersbn makes.
Its a little dirty, and eventually this should be in the sameersbn/gitlab repo instead.

To enable Google auth, just use this container (it uses "FROM sameersbn/gitlab"), and set the parameters:

* GITLAB_GOOGLE_AUTH_ENABLED to true
* GITLAB_GOOGLE_AUTH_APP_ID to your google auth app id (app_id)
* GITLAB_GOOGLE_AUTH_APP_SECRET to the app_secret

See https://gitlab.com/gitlab-org/gitlab-ce/blob/master/doc/integration/google.md for more info, or https://github.com/sameersbn/docker-gitlab/blob/master/assets/config/gitlabhq/gitlab.yml for the file need to modify.
