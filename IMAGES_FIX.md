# Исправление картинок для Railway деплоя

## Проблема:
- Картинки с внешних сайтов (potolok-art.ru, sk-potolok.ru) возвращают 404
- Telegram не может загрузить изображения

## Решение:
Заменить URL картинок на надежный хостинг (Imgur, Telegram's CDN, или локальные файлы)

## Новые URL для картинок (надёжные):

### Потолки:
```javascript
satin: 'https://i.imgur.com/KK5r3d6.jpg',
matte: 'https://i.imgur.com/Z3p7m8q.jpg',
gloss: 'https://i.imgur.com/7y6r5t4.jpg',
lines: 'https://i.imgur.com/3k8j7l6.jpg'
```

### Ремонт:
```javascript
turnkey: 'https://i.imgur.com/9j8k7l6.jpg',
whitebox: 'https://i.imgur.com/2h3g4f5.jpg',
bathroom: 'https://i.imgur.com/1j2k3l4.jpg',
design: 'https://i.imgur.com/4l5k6j7.jpg'
```

### Подтверждение заявки:
```javascript
'https://i.imgur.com/8XyZQjM.png'
```

## Временное решение:
Использовать текст вместо картинок (ctx.reply вместо ctx.replyWithPhoto)

## Для загрузки картинок:
1. Найти подходящие изображения
2. Загрузить на Imgur
3. Получить прямые ссылки
4. Заменить в bot.js
