# Deeplinks



## discord

protocol: discord://

Примеры:

- https://discord.com/channels/721998527575883816/721998528196378625
- discord://discord.com/channels/721998527575883816/721998528196378625


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://discord.com/channels/721998527575883816/721998528196378625 | discord://discord.com/channels/721998527575883816/721998528196378625 |


## Instagram

protocol: Instagram://

Примеры:

- https://www.instagram.com/teslamotors/
- https://www.instagram.com/p/B4D2Zn0BXj7/
- https://instagram.com/tv/CDUYDsWpuMi/

> https://api.instagram.com/oembed/?url=https://www.instagram.com/p/B4D2Zn0BXj7/

| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://instagram.com/profile | instagram://user?username=profile |
| https://instagram.com/p/{post} | instagram://media?id={media-id} |
| https://instagram.com/tv/{tv}  | instagram://media?id=/{tv} |



## Telegram

protocol: tg://

| DESKTOP | DEEPLINK |
| ------ | ------ |
| t.me/{name} | tg://resolve?domain={name} |
| https://t.me/joinchat/{chat}  | tg://join?invite={chat} |


## ВКонтакте

protocol: vk://

Примеры:

- Ссылки на профиль: vk.com/{id or name}
- Ссылки на группу: vk.com/{group id or group name}
- Ссылки на пост группы: vk.com/{group id or group name}?w=wall-{post-key}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://vk.com/durov  | vk://vk.com/durov |
| https://vk.com/deeplinkr?w=wall-173890828_63  | vk://vk.com/deeplinkr?w=wall-173890828_63 |


## Facebook

protocol: fb://

Примеры:

- Ссылки на профиль: facebook.com/{profile}
- Ссылки на страницу: facebook.com/{page profile}
- Ссылки на группу: facebook.com/groups/{group}
- Ссылки на события: facebook.com/events/{event}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://www.facebook.com/Cristiano  | fb://page/?id=415712035190005 |
| https://www.facebook.com/groups/ElonMusk/ | fb://group/?id=415712035190005 |
| https://www.facebook.com/events/1821878574616559/  | fb://event?id=1821878574616559 |

> Для android и ios ссылки разные

Для определения deeplink необходимо загрузить страницу и найти meta теги, их может не быть
```
<meta property="al:android:url" content="fb://group/415712035190005" />
<meta property="al:ios:url" content="fb://group/?id=415712035190005" />
```



## Youtube

protocol: vnd.youtube://

Примеры:

- Ссылка на канал: youtube.com/channel/{channel}
- Ссылка на видео: youtube.com/watch?v={video}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://www.youtube.com/channel/UCDK5Vv_LpNFADYYMkD2P4yA  | vnd.youtube://www.youtube.com/channel/UCDK5Vv_LpNFADYYMkD2P4yA |
| https://www.youtube.com/watch?v=dwkEYrE8hCI | vnd.youtube://www.youtube.com/watch?v=dwkEYrE8hCI |


## Twitter

protocol: twitter://

Примеры:

- Ссылки на профиль: twitter.com/{profile}
- Ссылки на пост: twitter.com/{profile}/status/{post_id}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://twitter.com/mancity  | twitter://user?screen_name=mancity |
| https://twitter.com/ManCity/status/1195303184480317440 | twitter://status?id=1195303184480317440 |


## TikTok

protocol: snssdk1233://

Примеры:

- Ссылки на профиль: vm.tiktok.com/{profile}
- Ссылки на видео: vm.tiktok.com/{video}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://vm.tiktok.com/J2VgmA5/  | snssdk1233://user/profile/6753638085679907845 |
| https://vm.tiktok.com/J2VG5cj/ | snssdk1233://vm.tiktok.com/video/6845595253706067206 |


Для определения deeplink необходимо загрузить страницу и найти meta теги, их может не быть
```
<meta property="al:android:url" content="snssdk1233://user/profile/6753638085679907845?refer=facebook">
<meta property="al:ios:url" content="snssdk1233://user/profile/6753638085679907845?refer=facebook">
```



## Spotify

protocol: spotify://

Примеры:

- Ссылки на альбом: open.spotify.com/album/{album}
- Ссылки на исполнителя: open.spotify.com/artist/{artist}
- Ссылки на плейлист: open.spotify.com/playlist/{playlist}
- Ссылки на трек: open.spotify.com/track/{track}
- Ссылки на подкаст (на данный момент не поддерживаются в Российском spotify): open.spotify.com/show/{show}


| DESKTOP | DEEPLINK |
| ------ | ------ |
| https://open.spotify.com/album/7CGhx630DIjdJqaBDVKc5j  | spotify://album/7CGhx630DIjdJqaBDVKc5j |
| https://open.spotify.com/artist/7dGJo4pcD2V6oG8kP0tJRR?si=WNOGt8_QQFe7-m6MzpwW5Q | spotify://artist/7dGJo4pcD2V6oG8kP0tJRR |
| https://open.spotify.com/playlist/4sNgAu89gfGRJD6NhyNvnK?si=LTLVaeuvQMex35YM8uG0pg | spotify://playlist/4sNgAu89gfGRJD6NhyNvnK |
| https://open.spotify.com/track/4oeaIftdpT3JuZLcCkKmVE?si=s__xVY0eQbmFqmeI8lWiYA | spotify://track/4oeaIftdpT3JuZLcCkKmVE |


