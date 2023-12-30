## Nano Api 
 
## Support Parameters  in header Request 

### header Request  Parameters

| Key                  | Type      | Description                                                  |
| -------------------- | --------- | ------------------------------------------------------------ |
| `Authorization`           | `string`  |  The token user  login   |
| `Accept-Language`           | `string`  |  The Locale Language  |


#### The Accept-Language 

**يمكن تهية اللغة فى النظام من خلال  تمرير كود اللغه فى راس الطلب ضمن المتغير  Accept-Language**

Header Parameters
```json
{
  "Accept-Language":"ar"
}
```

**عند تمرير المتغير السابق فى راس الطلب فان النظام سيقوم بجلب اي بيانات بالاعتماد على اللغه الممرره فمثلا لوقمن بتمرير كود اللغه العربيه سيتم ارجاع البيانات باللغه العربيه وهكذا**


## Support Response Type in Api 

### 1 ArraySerializer deafult
#### Example return ArraySerializer

```json
{
  "data": [
    {
      "id": 4,
      "code": "2-2-4",
      "barcode": "2-4",
      "name": "حبة دجاج برست",
      "emblem": "",
      "short_description": "",
      "description": "",
      "users_manual": "",
      "composition": "",
      "indication": "",
      "meta_title": "",
      "meta_description": "",
      "keywords": "",
      "ref_type_class": "products",
      "ref_key_values_class": "3",
      "groups_products_id": "2",
      "companys_id": "2",
      "departments_id": "2",
      "is_effective": 1,
      "is_default": null,
      "is_active": 1,
      "is_published": 1,
      "published_at": "",
      "unpublished_at": "",
      "manage_stock": 0,
      "shop_stock": 0,
      "min_qty": 1,
      "max_qty": 1,
      "min_qty_in_stock": 1,
      "max_qty_in_stock": 1,
      "default_qty": 1,
      "old_price": null,
      "price": 0,
      "is_show_old_price": 1,
      "is_parleying": 1,
      "is_sold": 1,
      "is_purchased": 1,
      "is_composite": 0,
      "is_units": 1,
      "is_downloadable": 1,
      "properties": null,
      "links": null,
      "other_data": null,
      "config_data": null,
      "sort_order": 4,
      "created_at": "2022-10-02 15:22:20",
      "updated_at": "2022-10-02 15:22:20",
      "image": {
        "original": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/633b47a8bee36870039097.png",
        "small": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_160_160_0_0_crop.png",
        "medium": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_240_240_0_0_crop.png",
        "large": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_800_800_0_0_crop.png",
        "thumb": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_480_480_0_0_auto.png"
      },
      "images": [],
      "files": [],
      "ratings_count": 4,
      "countRating": 4,
      "sumRating": "13",
      "averageRating": "3.2500",
      "user_is_rating": true,
      "user_object_rating": {
        "id": 15,
        "code": "2-4-15",
        "is_recommended": true,
        "rating": 3,
        "title": "543منتج رائع",
        "content": "التعليق 543",
        "approved": true,
        "reviewrateable_type": "products",
        "reviewrateable_id": 4,
        "user_type": "RainLab\\User\\Models\\User",
        "user_id": 543,
        "name": null,
        "email": null,
        "url": "\/api\/v1\/shop\/products",
        "hash": "8a20d49df9a87ab7c4fe945097bcca27",
        "locale": "ar",
        "ip": "127.0.0.1",
        "ip_forwarded": null,
        "user_agent": "okhttp\/3.8.1",
        "companys_id": "2",
        "departments_id": "4",
        "is_active": true,
        "other_data": null,
        "config_data": null,
        "sort_order": 15,
        "created_by": null,
        "updated_by": null,
        "deleted_by": null,
        "created_at": "2022-10-11 19:12:46",
        "updated_at": "2022-10-11 19:23:31",
        "deleted_at": null
      },
      "favorites_count": 3,
      "user_is_favorite": true,
      "user_object_favorite": {
        "user_id": 543,
        "favoriteable_type": "products",
        "favoriteable_id": 4,
        "created_at": "2022-10-09 23:46:35",
        "updated_at": "2022-10-09 23:46:35"
      },
      "categories": {
        "data": [
          {
            "id": 1,
            "code": "2-4-1",
            "name": "عامه",
            "slug": "aaamh",
            "type": "1",
            "user_id": null,
            "user_type": null,
            "companys_id": "2",
            "departments_id": "4",
            "country_id": null,
            "is_public": 1,
            "is_default": 0,
            "is_active": 1,
            "is_published": 1,
            "published_at": "",
            "unpublished_at": "",
            "main_sub": "main",
            "parent_id": null,
            "level": "1",
            "properties": null,
            "created_at": "2022-09-26 19:55:19",
            "updated_at": "2022-10-03 20:13:13"
          }
        ]
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 1,
      "count": 1,
      "per_page": 15,
      "current_page": 1,
      "total_pages": 1,
      "links": []
    }
  }
}
```

### 2 JsonApiSerializer
#### Example return JsonApiSerializer

```json
{
  "data": [
    {
      "type": null,
      "id": "4",
      "attributes": {
        "code": "2-2-4",
        "barcode": "2-4",
        "name": "حبة دجاج برست",
        "emblem": "",
        "short_description": "",
        "description": "",
        "users_manual": "",
        "composition": "",
        "indication": "",
        "meta_title": "",
        "meta_description": "",
        "keywords": "",
        "ref_type_class": "products",
        "ref_key_values_class": "3",
        "groups_products_id": "2",
        "companys_id": "2",
        "departments_id": "2",
        "is_effective": 1,
        "is_default": null,
        "is_active": 1,
        "is_published": 1,
        "published_at": "",
        "unpublished_at": "",
        "manage_stock": 0,
        "shop_stock": 0,
        "min_qty": 1,
        "max_qty": 1,
        "min_qty_in_stock": 1,
        "max_qty_in_stock": 1,
        "default_qty": 1,
        "old_price": null,
        "price": 0,
        "is_show_old_price": 1,
        "is_parleying": 1,
        "is_sold": 1,
        "is_purchased": 1,
        "is_composite": 0,
        "is_units": 1,
        "is_downloadable": 1,
        "properties": null,
        "links": null,
        "other_data": null,
        "config_data": null,
        "sort_order": 4,
        "created_at": "2022-10-02 15:22:20",
        "updated_at": "2022-10-02 15:22:20",
        "image": {
          "original": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/633b47a8bee36870039097.png",
          "small": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_160_160_0_0_crop.png",
          "medium": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_240_240_0_0_crop.png",
          "large": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_800_800_0_0_crop.png",
          "thumb": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_480_480_0_0_auto.png"
        },
        "images": [],
        "files": [],
        "ratings_count": 4,
        "countRating": 4,
        "sumRating": "13",
        "averageRating": "3.2500",
        "user_is_rating": true,
        "user_object_rating": {
          "id": 15,
          "code": "2-4-15",
          "is_recommended": true,
          "rating": 3,
          "title": "543منتج رائع",
          "content": "التعليق 543",
          "approved": true,
          "reviewrateable_type": "products",
          "reviewrateable_id": 4,
          "user_type": "RainLab\\User\\Models\\User",
          "user_id": 543,
          "name": null,
          "email": null,
          "url": "\/api\/v1\/shop\/products",
          "hash": "8a20d49df9a87ab7c4fe945097bcca27",
          "locale": "ar",
          "ip": "127.0.0.1",
          "ip_forwarded": null,
          "user_agent": "okhttp\/3.8.1",
          "companys_id": "2",
          "departments_id": "4",
          "is_active": true,
          "other_data": null,
          "config_data": null,
          "sort_order": 15,
          "created_by": null,
          "updated_by": null,
          "deleted_by": null,
          "created_at": "2022-10-11 19:12:46",
          "updated_at": "2022-10-11 19:23:31",
          "deleted_at": null
        },
        "favorites_count": 3,
        "user_is_favorite": true,
        "user_object_favorite": {
          "user_id": 543,
          "favoriteable_type": "products",
          "favoriteable_id": 4,
          "created_at": "2022-10-09 23:46:35",
          "updated_at": "2022-10-09 23:46:35"
        }
      },
      "relationships": {
        "categories": {
          "data": [
            {
              "type": null,
              "id": "1"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "type": null,
      "id": "1",
      "attributes": {
        "code": "2-4-1",
        "name": "عامه",
        "slug": "aaamh",
        "type": "1",
        "user_id": null,
        "user_type": null,
        "companys_id": "2",
        "departments_id": "4",
        "country_id": null,
        "is_public": 1,
        "is_default": 0,
        "is_active": 1,
        "is_published": 1,
        "published_at": "",
        "unpublished_at": "",
        "main_sub": "main",
        "parent_id": null,
        "level": "1",
        "properties": null,
        "created_at": "2022-09-26 19:55:19",
        "updated_at": "2022-10-03 20:13:13"
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 1,
      "count": 1,
      "per_page": 15,
      "current_page": 1,
      "total_pages": 1
    }
  },
  "links": {
    "self": "http:\/\/localhost:8006\/api\/v1\/shop\/products?page=1",
    "first": "http:\/\/localhost:8006\/api\/v1\/shop\/products?page=1",
    "last": "http:\/\/localhost:8006\/api\/v1\/shop\/products?page=1"
  }
}
```


### 3 DataArraySerializer
#### Example return DataArraySerializer

```json
{
  "data": [
    {
      "id": 4,
      "code": "2-2-4",
      "barcode": "2-4",
      "name": "حبة دجاج برست",
      "emblem": "",
      "short_description": "",
      "description": "",
      "users_manual": "",
      "composition": "",
      "indication": "",
      "meta_title": "",
      "meta_description": "",
      "keywords": "",
      "ref_type_class": "products",
      "ref_key_values_class": "3",
      "groups_products_id": "2",
      "companys_id": "2",
      "departments_id": "2",
      "is_effective": 1,
      "is_default": null,
      "is_active": 1,
      "is_published": 1,
      "published_at": "",
      "unpublished_at": "",
      "manage_stock": 0,
      "shop_stock": 0,
      "min_qty": 1,
      "max_qty": 1,
      "min_qty_in_stock": 1,
      "max_qty_in_stock": 1,
      "default_qty": 1,
      "old_price": null,
      "price": 0,
      "is_show_old_price": 1,
      "is_parleying": 1,
      "is_sold": 1,
      "is_purchased": 1,
      "is_composite": 0,
      "is_units": 1,
      "is_downloadable": 1,
      "properties": null,
      "links": null,
      "other_data": null,
      "config_data": null,
      "sort_order": 4,
      "created_at": "2022-10-02 15:22:20",
      "updated_at": "2022-10-02 15:22:20",
      "image": {
        "original": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/633b47a8bee36870039097.png",
        "small": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_160_160_0_0_crop.png",
        "medium": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_240_240_0_0_crop.png",
        "large": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_800_800_0_0_crop.png",
        "thumb": "http:\/\/localhost:8006\/storage\/app\/uploads\/public\/633\/b47\/a8b\/thumb_567_480_480_0_0_auto.png"
      },
      "images": [],
      "files": [],
      "ratings_count": 4,
      "countRating": 4,
      "sumRating": "13",
      "averageRating": "3.2500",
      "user_is_rating": true,
      "user_object_rating": {
        "id": 15,
        "code": "2-4-15",
        "is_recommended": true,
        "rating": 3,
        "title": "543منتج رائع",
        "content": "التعليق 543",
        "approved": true,
        "reviewrateable_type": "products",
        "reviewrateable_id": 4,
        "user_type": "RainLab\\User\\Models\\User",
        "user_id": 543,
        "name": null,
        "email": null,
        "url": "\/api\/v1\/shop\/products",
        "hash": "8a20d49df9a87ab7c4fe945097bcca27",
        "locale": "ar",
        "ip": "127.0.0.1",
        "ip_forwarded": null,
        "user_agent": "okhttp\/3.8.1",
        "companys_id": "2",
        "departments_id": "4",
        "is_active": true,
        "other_data": null,
        "config_data": null,
        "sort_order": 15,
        "created_by": null,
        "updated_by": null,
        "deleted_by": null,
        "created_at": "2022-10-11 19:12:46",
        "updated_at": "2022-10-11 19:23:31",
        "deleted_at": null
      },
      "favorites_count": 3,
      "user_is_favorite": true,
      "user_object_favorite": {
        "user_id": 543,
        "favoriteable_type": "products",
        "favoriteable_id": 4,
        "created_at": "2022-10-09 23:46:35",
        "updated_at": "2022-10-09 23:46:35"
      },
      "categories": {
        "data": [
          {
            "id": 1,
            "code": "2-4-1",
            "name": "عامه",
            "slug": "aaamh",
            "type": "1",
            "user_id": null,
            "user_type": null,
            "companys_id": "2",
            "departments_id": "4",
            "country_id": null,
            "is_public": 1,
            "is_default": 0,
            "is_active": 1,
            "is_published": 1,
            "published_at": "",
            "unpublished_at": "",
            "main_sub": "main",
            "parent_id": null,
            "level": "1",
            "properties": null,
            "created_at": "2022-09-26 19:55:19",
            "updated_at": "2022-10-03 20:13:13"
          }
        ]
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 1,
      "count": 1,
      "per_page": 15,
      "current_page": 1,
      "total_pages": 1,
      "links": []
    }
  }
}
```

### Public Parameters
| Key                  | Type      | Description                                                  |
| -------------------- | --------- | ------------------------------------------------------------ |
| `q`           | `string`  |  using search in departments records |
| `orderBy`           | `string`  |  using orderBy departments records - Name column default value created_at |
| `orderDirection`           | `string`  |  using orderBy departments records [asc,desc] - Name column default value desc |
| `per_page`           | `integer`  |  Number Records in Page default value 15 |
| `page`           | `integer`  |  Number  Page default value 1 |
| `include`           | `string` | get relation using [relation1,relation2,relation3]
| 

#### Include Relation 

| Relation Name                  | Type      | Description                                                  |
| -------------------- | --------- | ------------------------------------------------------------ |
| `companys`           | `belongsTo`  | The get companys |
| `tags_type`           | `belongsTo`  | The get Type Refrence | 
| `parent`           | `belongsTo`  | The get parent departments   | 
| `children`           | `hasMany`  | The get childrens departments   | 
| `country`           | `belongsTo`  | The get country data   | 
| `state`           | `belongsTo`  | The get state data   | 
| `directorate`           | `belongsTo`  | The get directorate data   | 
