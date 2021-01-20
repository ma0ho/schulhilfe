# Schulhilfe

This repository bundles a Wordpress instance and a Zammad ticket system using docker compose. It is part of the project "Schulhilfe", which aims at helping schools during the COVID-19 pandemic.

## Setup

### Step 1:

Modify configuration in ```.env``` to suit your needs. Please make sure to set the passwords to random ones.

### Step 2:

Put certificates and keys under ```ssl/```. For every domain, you need a ```domainname.key``` and a ```domainname.crt``` file. Here, you replace ```domainname``` with the actual domain name. For example, the certificate for ```news.schulhilfe.fau.de``` is ```news.schulhilfe.fau.de.crt```.

## Startup

You may start the server by issueing

```bash
docker-compose up -d
```

on the command line. Later, you might check everything with

```bash
docker-compose ps
```