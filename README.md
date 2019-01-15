# WordPress Database Renamer
### Repository: wp_db_rename
SQL statements to correctly rename the prefix of a WordPress database.

Change all Database Tables Name

```shell
RENAME table `wp_commentmeta` TO `xxx_commentmeta`;
RENAME table `wp_comments` TO `xxx_comments`;
RENAME table `wp_links` TO `xxx_links`;
RENAME table `wp_options` TO `xxx_options`;
RENAME table `wp_postmeta` TO `xxx_postmeta`;
RENAME table `wp_posts` TO `xxx_posts`;
RENAME table `wp_terms` TO `xxx_terms`;
RENAME table `wp_termmeta` TO `xxx_termmeta`;
RENAME table `wp_term_relationships` TO `xxx_term_relationships`;
RENAME table `wp_term_taxonomy` TO `xxx_term_taxonomy`;
RENAME table `wp_usermeta` TO `xxx_usermeta`;
RENAME table `wp_users` TO `xxx_users`;
```

The Options Table

```shell
SELECT * FROM `xxx_options` WHERE `option_name` LIKE '%wp_%'
```

UserMeta Table

```shell
SELECT * FROM `xxx_usermeta` WHERE `meta_key` LIKE '%wp_%'
```
