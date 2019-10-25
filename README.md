# HabboAPI v.3.3.6
Documentation: [HabboAPI Website](https://habboapi.net/).

- Over **60.000** Badges
- Over **6.500** Furniture
- Over **500** Clothing

Habbo API is a free to use API, that aim to help Habbo fansite builders create awesome tools and features for their fansites. We offer a large number of API endpoints, that serve you the lastest Habbo Badges, Furniture, Clothes and hopefully a lot more, in the future.

Twitter: [Official Twitter](https://twitter.com/habboapi).

## Authentication
To use our API you **dont need any authentication**. It's free to use, you just need to call our endpoint.

## Rate Limiting
There's **no** Rate-limiting enforced in our API.

## Endpoints
#### [badges](badges/README.md)
- [List badges](badges/get.md) : `GET /badges`
- [List single badges](badges/show.md) : `GET /badges/show.md` - _coming soon_
- [List badges by hotel](badges/hotel.md) : `GET /badges/hotel.md` - _coming soon_

#### [furni](furni/README.md)
- [List furnis](furni/get.md) : `GET /furni`
- [List single furni](furni/show.md) : `GET /furni/show.md` - _coming soon_
- [Use furni directions](furni/directions.md) : `GET /furni/directions.md` - _coming soon_
- [Use furni colors](furni/colors.md) : `GET /furni/colors.md` - _coming soon_

#### [clothing](clothing/README.md)
- [List clothing](clothing/get.md) : `GET /clothing`
- [List single clothing](clothing/show.md) : `GET /clothing/show.md` - _coming soon_
- [Use clothing directions](clothing/directions.md) : `GET /clothing/directions.md` - _coming soon_

## Credits
Made by [Incor](https://github.com/inctor) and [HabboAPI](https://github.com/habboapi).

## Changelog
- **September 2019**
  - > **3.3.6** | Added _badge_owners_ to `/badges`
  - > **3.3.6** | Fixed missing furni `/furni`
- **April 2019**
  - > **3.3.5** | Added _states_ to `/furni`
