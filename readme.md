## Laravel 5.4 Realtime Chat + Pusher

This app was based on this tutorial: https://blog.pusher.com/how-to-build-a-laravel-chat-app-with-pusher/

### Running

- Create a free account in [Pusher](https://pusher.com/signup)


- Create an app in Pusher and get the keys


- In your `.env` setup the Pusher keys:
```
BROADCAST_DRIVER=pusher
PUSHER_APP_ID=YOUR_APP_ID
PUSHER_APP_KEY=YOUR_APP_KEY
PUSHER_APP_SECRET=YOUR_APP_SECRET
PUSHER_CLUSTER=YOUR_PUSHER_CLUSTER
```


- In `resources/assets/js/bootstrap.js` line 47, replace the `PUSHER_APP_KEY` and `PUSHER_CLUSTER` to your to your respective Pusher values.


- Now, follow this steps:
```bash

# Install Laravel dependencies
composer install

# Install Node dependencies
npm install

# Configure your database and run the migrations
php artisan migrate

# Compile the JavaScript files using Laravel Mix
npm run dev

# Start the chat app
php artisan serve
```

Enjoy :)


License: [BSD 3-Clause](LICENSE)


<a href='https://ko-fi.com/N4N09BMZ' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi1.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
