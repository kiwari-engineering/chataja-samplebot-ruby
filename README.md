# Kiwari Bot Webhook Sample with Ruby

## Requirements

* [Ruby](https://www.ruby-lang.org/en/)
* [Ruby on Rails](https://rubyonrails.org/)
* [Bundler](https://bundler.io/bundle_install.html)
* [ngrok](https://ngrok.com/)
* Bot Access Token (you can chat with Chatbot Builder in `Jelajah` menu)

## How to run

* Clone this repository and install dependencies `Gemfile`

```bash
$ git clone https://gitlab.playcourt.id/iskandarsuhaimi/webhook-kiwaribot-sample-ruby.git
$ cd webhook-kiwaribot-sample-ruby
$ bundle install
```

* Go to `Jelajah` menu
* chat with `Chatbot Builder`
* Create bot and get `access_token`
* Copy and Paste to `chat_controller.rb` class

* Run webhook server

```bash
$ rake db:create db:migrate
$ rails server
```

* Tunneling your webhook server

```bash
$ ngrok http 3000
```

* Register your webhook url by copy your ngrok https url from CLI, then input it to `Chatbot Builder`
* Enjoy!