# Jellyfin Webhook Plugin 
## Part of the [Jellyfin Project](https://jellyfin.org)

#### Repository - https://repo.codyrobibero.dev/manifest.json

Use [Handlebars](https://handlebarsjs.com/guide/) templating engine to format notifications however you wish.

See [Templates](Jellyfin.Plugin.Webhook/Templates) for sample templates.

#### Helpers:

- if_equals
    - if first parameter equals second parameter case insensitive
- if_exist
    - if the value of the parameter is not null or empty
- link_to
    - wrap the $url and $text in an `<a>` tag

#### Variables:

- Generic:
    - Timestamp (Current server time local)
    - UtcTimestamp (Current server time utc)
    - Name (Item name)
    - Overview (Item overview)
    - ItemId (Item id)
    - ServerId (Server id)
    - ServerUrl (Server url)
    - ServerName (Server name)
    - ItemType (Item type)
    - Year (Item production year)
    - SeriesName (TV series name)
    - SeasonNumber (Series number - direct format)
    - SeasonNumber00 (Series number - padded 00)
    - SeasonNumber000 (Series number - padded 000)
    - EpisodeNumber (Episode number - direct format)
    - EpisodeNumber00 (Episode number - padded 00)
    - EpisodeNumber000 (Episode number - padded 000)
    - Provider_{providerId_lowercase} (ProviderId is lowercase)

- Discord
    - MentionType
    - EmbedColor
    - AvatarUrl
    - Username
- Gotify
    - Priority
- Pushover
    - Token
    - UserToken
    - Device
    - Title
    - MessageUrl
    - MessageUrlTitle
    - MessagePriority
    - NotificationSound

- Destinations:
    - Discord
    - Gotify
    - Pushover
    - Generic


- TODO
    - Pushbullet
    - Prowl
    - Teli?
