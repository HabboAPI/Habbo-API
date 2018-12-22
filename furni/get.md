# Shows all furni
Lists all furnis that we have scanned and registered.

**URL**: `/furni`

**Method**: `GET`

**Parameters**

| Name | In | Type | Required | Details |
| --- | --- | --- | --- | --- |
| per_page | Query | Integer (Default: `50`) | No | Paginates the result by value provided |
| name | Query | String | No | Wildcard search for furni with that name |
| description | Query | String | No | Wildcard search for furni with that description |
| code | Query | String | No | Wildcard search for furni with that code |
| habbo_furni_id | Query | String | No | Wildcard search for furni with that habbo furni id |
| line | Query | String | No | Wildcard search for furni with that line-code |
| for_sale | Query | String | No | If supplied, will only return `for_sale` furni |
| builders_club | Query | String | No | If supplied, will only return `builders_club` furni |
| new | Query | String | No | If supplied, will only return `new` furni |

## Request example
**Return a list of all furnis in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/furni' \
  --header 'Content-Type: application/json'
```

**Return a list of all new furni in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/furni?new=true' \
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
         "id":6443,
         "name":"year2019 name",
         "code":"year2019",
         "description":"year2019 desc",
         "habbo_furni_id":4683,
         "furni_line":"newyear_2019",
         "furni_line_name":"newyear_2019",
         "image":"https://api.socialhabbo.com/furni/year2019/image",
         "icon":"https://api.socialhabbo.com/furni/year2019/icon",
         "public_icon":"http://habboo-a.akamaihd.net/dcr/hof_furni/64583/year2019_icon.png",
         "colors":[

         ],
         "directions":[
            {
               "direction_id":2,
               "image":"https://api.socialhabbo.com/furni/year2019/image?direction=2"
            },
            {
               "direction_id":4,
               "image":"https://api.socialhabbo.com/furni/year2019/image?direction=4"
            }
         ],
         "states":[
            {
               "state_id":0,
               "image":"https://api.socialhabbo.com/furni/year2019/image?state=0"
            },
            {
               "state_id":1,
               "image":"https://api.socialhabbo.com/furni/year2019/image?state=1"
            },
            {
               "state_id":100,
               "image":"https://api.socialhabbo.com/furni/year2019/image?state=100"
            }
         ],
         "for_sale":false,
         "builders_club":false,
         "discovered_at":"2018-12-13 16:41:56",
         "discovered_at_iso":"2018-12-13T16:41:56+00:00",
         "new":false
      }
   ],
   "from":1,
   "last_page":122,
   "next_page_url":"https://api.socialhabbo.com/furni?page=2",
   "path":"https://api.socialhabbo.com/furni",
   "per_page":50,
   "prev_page_url":null,
   "to":50,
   "total":6064
}
```
