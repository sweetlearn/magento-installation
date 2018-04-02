# Magento 2 theme installation
Setps for install theme to magento 2 
### install theme files to root of magento dircetory

#### Disable all cache related section that you have in your magento.

```shell
bin/magento cache:disable
```

#### Enable or disable cache types

Just example 
             bin/magento cache:enable [type] ... [type]
             bin/magento cache:disable [type] ... [type]

### View the cache status :

```shell
bin/magento cache:status
```
A sample just like follows:

              config: 1
            layout: 1
        block_html: 1
       collections: 1
            db_ddl: 1
               eav: 1
         full_page: 1
         translate: 1
config_integration: 1 config_integration_api: 1
 config_webservice: 1
  
  --- OR ---
  
  Changed cache status:
                    db_ddl: 1 -> 0
                 full_page: 1 -> 0
                 

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





