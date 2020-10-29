# SSO Example

This repo contains the final configuration files for setting up SSO with Auth0, nginx, and vouch-proxy. It is meant to be run inside docker.

For a full article on how to configure a web app using these services, see the accompanying article:

https://sebastianwallkoetter.wordpress.com/2020/10/29/sso-for-your-app/

### How to run

1. Replace the placeholder fields `your-project-name-here`, `{client_id_from_auth0}`, `{client_secret_from_auth0}` with the correct values.
2. Navigate into the `cert` folder and generate a pair of SSL certificates via `docker run --rm -it -v$PWD:/certs firefoxmetzger/create_localhost_ssl` (check https://github.com/FirefoxMetzger/create_ssl) for details.
3. `docker-compose up`

Please have a look at the acompanying article first if you struggle setting things up. Otherwise, if you have trouble or find a problem/bug, open an issue =).
