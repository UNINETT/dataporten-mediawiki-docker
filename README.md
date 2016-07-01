# dataporten-mediawiki-docker

This is a oAuth2.0 plugin for MediaWiki with Dataporten. 

1 - To run it with docker, run

```$ docker pull uninettno/dataporten-mediawiki-docker```

2 - Create an env.list:

```
DATAPORTEN_CLIENTID=*******
DATAPORTEN_CLIENTSECRET=******
DATAPORTEN_RIGHTS_ARRAY={"fc:org:uninett.no:unit:SEL-S": "user", "fc:org:uninett.no":"sysop"}

MEDIAWIKI_SITE_SERVER=******
MEDIAWIKI_RESTBASE_URL=******
MEDIAWIKI_DB_TYPE=******
MEDIAWIKI_DB_HOST=*****
MEDIAWIKI_DB_USER=*****
MEDIAWIKI_DB_PASSWORD=*****
MEDIAWIKI_DB_NAME=*****

MEDIAWIKI_SITE_NAME=*****
MEDIAWIKI_SITE_LANG=*****
MEDIAWIKI_ADMIN_USER=*****
MEDIAWIKI_ADMIN_PASS=*****

```

3 - Start the image with:

```$ docker run --env-file=YOUR_ENV_FILE -p DESIRED_PORT:80 -t uninettno/dataporten-mediawiki-docker```

