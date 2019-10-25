# Shows all badges
Lists all badges that we have scanned and registered.

**URL**: `/badges`

**Method**: `GET`

**Parameters**

| Name | In | Type | Required | Details |
| --- | --- | --- | --- | --- |
| per_page | Query | Integer (Default: `50`) | No | Paginates the result by value provided |
| name | Query | String | No | Wildcard search for badges with that name |
| description | Query | String | No | Wildcard search for badges with that description |
| code | Query | String | No | Wildcard search for badges with that code |
| hotel | Query | String | No | Wildcard search for badges for specific hotel only |
| achievement | Query | String | No | Wildcard search for achievement badges |
| has_image | Query | String | No | If supplied, will only return badges with image |
| new | Query | String | No | If supplied, will only return `new` badges |

## Request example
**Return a list of all badges in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/badges' \
  --header 'Content-Type: application/json'
```

**Return a list of all new badges in the API**
```bash
curl --request GET \
  --url 'https://api.socialhabbo.com/badges?new=true' \
  --header 'Content-Type: application/json'
```

## Success Response
**Code**: `200 OK`

**Content-Type**: `application/json`

**Content**
```json
{
   current_page: 1,
   data: [
      {
         code: "TRE30",
         name: "Habboloji.com / Şu Surata Bir Gülümseme Yerleştirelim",
         description: "",
         hotel: "com.tr",
         discovered_at_iso: "2019-10-25T13:37:10+00:00",
         discovered_at: "2019-10-25 13:37:10",
         image: "https://habboo-a.akamaihd.net/c_images/album1584/TRE30.gif",
         achievement: false,
         new: true,
         has_image: true,
         badge_owners: 0,
      }
   ],
   from: 1,
   last_page: 58604,
   next_page_url: "https://api.habboapi.net/badges?page=2",
   path: "https://api.habboapi.net/badges",
   per_page: "1",
   prev_page_url: null,
   to: 1,
   total: 58604,
}
```
