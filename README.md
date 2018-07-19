# docker-wpupdate
docker-compose to auto update wpcore

## Usage
1. copy docker-compose.yml to wp webroot
2. run `docker-compose -p wp -f docker-compose-wpupdate.yml up -d`
3. watch the logs: `docker logs -f wp_cli_1`

## Misc
* Haven't figured this out yet, wp-config.php get's updated to environment creds.  Revert the changes in git:
  1. `git diff --name-only`
  2. `git checkout HEAD -- wp-config.php`
  
