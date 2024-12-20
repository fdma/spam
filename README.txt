
Комментарии Спам-бот

# Больше схем на SEOCHAO.RU

Бот максимально быстро пишет указанные сообщения в комментариях к новым публикациям, или как мы его называем - Бот-первонах.


Installation 
```
pip install -r requirements.txt
python userbot.py
```
Не забудьте настроить файл data/config.ini и переменные в userbot.py - это те самые API и HASH из самой схемы.

Delay
Delay = 0,25. Вы можете увеличить задержку между взаимодействиями с серверами Telegram, если ваша учетная запись быстро умирает.


Типы сообщений:


1)Текст:

Синтаксис: spam_posts = [TextPost("текст")]
Пример:
 spam_posts = [TextPost("Кто такой Брюховецкий куколд Ваня Каушан?")]

Многострочный пример:
 spam_posts = [TextPost("""
Это будет в первой строке
Это будет на второй линии
Это будет на третьей линии
""")]

2)Изображение

Файл изображения должен находиться в одном каталоге с userbot.py. 
Синтаксис: spam_posts = [PicturePost("фото", "подпись")]
Пример:
 spam_posts = [PicturePost("nat.jpg", "Красивая природа! 😉")]


3)Стикер:

Вы можете получить идентификатор стикера здесь: https://t.me/sticker_file_id_bot
Синтаксис: spam_posts = [StickerPost("sticker_id")]
Пример:
 spam_posts = [StickerPost("CAACAgIAAxkBAAL6PGIzHXlhIR_MIRDaXz116O2Ic8AAJpAAOmysgM41g56v0Hj1wjBA")]


4)Случайное сообщение

Синтаксис: spam_posts = [RandomPost(сообщения))]
Пример:
 spam_posts = [RandomPost(TextPost("Random 1"), TextPost("Random 2"))]


5)Мультипост

Синтаксис: spam_posts = [сообщения]
Пример:
 spam_posts = [TextPost("Немного текста!"), PicturePost("nat.jpg", "И красивая природа!")]


6)DelayedPost

Синтаксис: spam_posts = [post(..., delay=seconds)]
Пример:
spam_posts = [TextPost("1st!", delay=2), PicturePost("nature.jpg", "nature", delay=4)]



```Используемые модули Python
pyrogram=1.4.16
tgcrypto
```

ИЗИ
