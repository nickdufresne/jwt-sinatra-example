jwt-sinatra-example
===================

JSON Web Token authentication in sinatra example app

Helpful articles about JSON Web Token and ruby:

http://www.intridea.com/blog/2013/11/7/json-web-token-the-useful-little-standard-you-haven-t-heard-about

Built using:

[Sinatra](http://www.sinatrarb.com)

[ruby-jwt](https://github.com/progrium/ruby-jwt)

To get started with this project
=================================

Clone this repo and run bundle

To start the sinatra server:

from jwt-sinatra-example/

`ruby app.rb`

You should see sinatra fire up with Webrick.  Point your web browser to:

http://localhost:4567/

This app will load app.rsa and app.rsa.pub as sign and verify keys for the JWT encode and decode

the app.rsa and app.rsa.pub were generated with:

`openssl genrsa -out app.rsa 2048`

`openssl rsa -in app.rsa -pubout > app.rsa.pub`