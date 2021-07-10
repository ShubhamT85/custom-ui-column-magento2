# Magento 2(Custom UI column for products grid in admin)
This module will create a custom column in products grid to give stock management details.
## Basic Flow of the module
- Firstly, after cloning the git and extracting the folder wrap it inside folder **Custom** and again wrap this folder in **Task** so inshort, create your directory as magento-root-directory/app/code/Task/Custom/cloned_directory.
- After that open the magento root directory in terminal and hit the following commands,
  - `sudo php bin/magento module:enable Task_Custom`
  - `sudo php bin/magento setup:upgrade`
  - `sudo php bin/magento setup:di:compile`
  - `sudo php bin/magento setup:static-content:deploy -f`
  - `sudo php bin/magento indexer:reindex` (optional)
  - `sudo php bin/magento cache:flush`
  - `sudo chmod 777 -R var/ pub/ generated/`
- Now, open your web browser and type in the following link to open magento admin (assuming for localhost or else type in https://your-magento-from-ftp/admin) **localhost/magento-root-directory/admin** and then go to Catalog->Products, you will see a new column named **Manage Stock** which will contain data of stock management i.e. Yes OR No.
### Happy Coding :)


