---
title: A Guide to Sending Telegram Messages
description: >-
  A comprehensive guide to programmatically sending messages through Telegram's
  Bot API, including setup and implementation examples.
date: '2023-07-08'
---

1.  Start a conversation with @BotFather.
2.  Run the /newbot command.
3.  Choose a name for your bot and save the HTTP token that's provided.
4.  Since your browser can send HTTPS requests, you can quickly test the API. After obtaining your token, try pasting this string into your browser to get started:
5.  Find your chat ID in the list

```
https://api.telegram.org/bot<TOKEN>/getUpdates
```

6. Make a GET request to:

```
 https://api.telegram.org/bot{{ $json.bot_token }}/sendMessage?chat_id={{ $json.chat_id}}&parse_mode=html&text={{ $json.message }}
```

![](/images/nachoficate.png)