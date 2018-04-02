# Magento 2 theme installation
Setps for install theme to magento 2 
### install theme files to root of magento dircetory

Run shell commands

```shell
sudo  <Magento file directory>
```
## Setup Upgrade : 

```shell
bin/magento setup:upgrade
```
And wait ...

## Clean cache : 

```shell
bin/magento cache:clean
```

## Static deploy command :

```shell
bin/magento setup:static-content:deploy -f
```

## Move to magento admin :
Go to : CONTENT > DESIGN > THEMES > just to see your theme there 

## Configrations :

Go to : CONTENT > DESIGN > CONFIGRATION >

Click Edit ==== main website store 
Applied theme ==== chose your theme from list

## Clean the cache :

```shell
bin/magento cache:clean
```
## back to your website and open it :

Run this command to render static files

```shell
bin/magento setup:static-content:deploy -f
```
## Refresh your website again





