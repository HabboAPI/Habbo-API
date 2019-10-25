# Shows all Clothing
Lists all clothing that we have scanned and registered.

**URL**: `/clothing`

**Method**: `GET`

**Parameters**

| Name | In | Type | Required | Details |
| --- | --- | --- | --- | --- |
| per_page | Query | Integer (Default: `50`) | No | Paginates the result by value provided |
| name | Query | String | No | Wildcard search for clothing with that name |
| description | Query | String | No | Wildcard search for clothing with that description |
| code | Query | String | No | Wildcard search for clothing with that code |
| habbo_furni_id | Query | String | No | Wildcard search for clothing with that habbo furni id |
| furni_line | Query | String | No | Wildcard search for clothing with that line-code |
| for_sale | Query | String | No | If supplied, will only return `for_sale` clothing |ing |
| new | Query | String | No | If supplied, will only return `new` clothing |

## Request example
**Return a list of all clothing in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/clothing' \
  --header 'Content-Type: application/json'
```

**Return a list of all new clothing in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/clothing?new=true' \
  --header 'Content-Type: application/json'
```

## Success Response
**Code**: `200 OK`

**Content-Type**: `application/json`

**Content**
```json
{
   "current_page":1,
   "data":[
      {
         "name":"clothing_icecrown name",
         "code":"clothing_icecrown",
         "description":"clothing_icecrown desc",
         "habbo_furni_id":10944,
         "furni_line":"xmas2019",
         "furni_line_name":"xmas2019",
         "image":"https://api.socialhabbo.com/furni/clothing_icecrown/image",
         "icon":"https://api.socialhabbo.com/furni/clothing_icecrown/icon",
         "public_icon":"http://habboo-a.akamaihd.net/dcr/hof_furni/65312/clothing_icecrown_icon.png",
         "directions":[
            {
               "direction_id":0
            },
            {
               "direction_id":2
            },
         ],
         "for_sale":false,
         "discovered_at":"2019-10-21 13:41:33",
         "discovered_at_iso":"2019-10-21T13:41:33+00:00",
         "new":false,
      }
   ],
   "from":1,
   "last_page":494,
   "next_page_url":"https://api.habboapi.net/clothing?page=2",
   "path":"https://api.habboapi.net/clothing",
   "per_page":"1",
   "prev_page_url":null,
   "to":1,
   "total":494,
}
```
