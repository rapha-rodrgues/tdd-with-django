Provisionando um novo site
==========================

## Pacotes necessários

* Nginx
* Python 3.6+
* virtualenv + pip
* Git

## Config do Nginx no servidor

* veja nginx.template.conf
* substitua SITENAME, por exemplo, por staging.my-domain.com

## Serviço Systemd

* veja gunicorn-systemd.template.service
* substitua SITENAME, por exemplo, por staging.my-domain.com

## Estruta dos diretórios no servidor

```bash
/home/username
|-- sites
   |-- SITENAME
      |-- database
      |-- source
      |-- static
      |-- virtualenv
```