
A Sample application for Setting up Device gem along with Nify Generator Plugin

Ruby version: 1.9.2
Rails version: 3.2.7
Database: PostgresSQL
====================================================================================================

Added the following gems in the Gemfile:

1. gem "nifty-generators", :group => :development

2. gem 'devise'

3. gem 'tlsmail' (This is used by Device for sending mails)

4. gem 'pg' (Added this gem for PostgreSQL support)

You can clone it by and start the application by the following steps:

1. git clone git://github.com/csaurav/tutorial-device-nifty-generator.git your-direcotry
2. cd your-direcotry
3. bundle install
4. rake db:create (Change the database parameters according to your system)
5. rake db:migrate
6. rails server

If you want to deploy the application in Heroku, then inside the application.rb, you have to make the following changes:

config.assets.initialize_on_precompile = false








