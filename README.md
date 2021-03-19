First of all make sure you've created a rails app

```bash
rails new APP_NAME
```

## Setup

Replace Rails' pages by Ubi Innovation Team's default pages:

```
rm app/views/pages/home.html.erb
rm app/views/pages/welcome.html.erb
curl -L https://gitlab-ncsa.ubisoft.org/adhuy/rails-pages/-/raw/master/home.html.erb > app/views/pages/home.html.erb
curl -L https://gitlab-ncsa.ubisoft.org/adhuy/rails-pages/-/raw/master/welcome.html.erb > app/views/pages/welcome.html.erb
```


**On Ubuntu/Windows**: if the `unzip` command returns an error, please install it first by running `sudo apt install unzip`.

And the viewport in the layout

```html
<!-- app/views/layouts/application.html.erb -->
<head>
  <!-- Add these line for detecting device width -->
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">

  <!-- [...] -->
</head>
```
