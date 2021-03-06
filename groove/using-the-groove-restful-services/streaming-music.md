---
title: Stream music for a subscribed user | Groove Services
description: Users subscripted to Groove Music Pass can stream full music tracks from your application.
keywords: groove api, groove stream music, groove music streaming 
author: sakley
ms.assetid: 988202c1-efd7-d43b-ee7e-89b134c96c58
---

# Streaming music
To stream a full music track you need an authenticated user with an active Groove Music Pass subscription.
See [User Authentication] for more details on how to authenticate users.
Once you have a user token, you should check if the user has an active Groove Music subscription. See [/1/user/music/profile].
If the user has a subscription, you can stream full music tracks. See [/1/content/{id}/stream].

If the user doesn't have a subscription or no user is signed-in, you can get access to a 30-second sample of all the music tracks. See [/1/content/{id}/preview].

30-second samples are in mp3 format.
OneDrive content is in its source format (whatever the user uploaded to his OneDrive storage).
Catalog full music tracks are in HLS format.
Refer to the stream APIs for more details: [/1/content/{id}/stream].

[/1/content/{id}/preview]: ../Groove-service-REST-Reference/uri-get-preview.md
[/1/content/{id}/stream]: ../Groove-service-REST-Reference/uri-get-stream.md
[User Authentication]: User-Authentication.md
