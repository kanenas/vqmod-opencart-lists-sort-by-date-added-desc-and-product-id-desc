# [VQMOD] Mixed lists with default sort order by date_added DESC AND product_id DESC in all lists

**Opencart**: v.2.1.x  
**Attention**: You have to install `[VQMOD]` for **Opencart** ( https://github.com/vqmod/vqmod/releases ) for this to work!

Upload the content of the `upload` folder.
```
CREATE TABLE `gnrctbl_product_to_category_custom_order` (
 `product_id` int(11) NOT NULL,
 `category_id` int(11) NOT NULL,
 `custom_order_id` int(11) NOT NULL,
 PRIMARY KEY (`product_id`,`category_id`) USING BTREE,
 KEY `category_id` (`category_id`) USING BTREE
) ENGINE=InnoDB DEFAULT CHARSET=utf8
```
