# Sound Objects Platform Server

This repo contains the Sound Objects Platform Server, which consists of:

* Website CMS for soundobjects.xyz
* Microservices for various API endpoints
* Models and Controllers to support the microservices

## Technology Stack (pre-requisites)

* Git | Code version control
* Rbenv v1.2.0 | Ruby version management
* Ruby v3.1.3 | Ruby language
* Rails v7.0.4.2 | Rails Web Framework
* PostgreSQL v14 | Backend Database

## Install Pre-requisites (Below instructions are for MacOS)

Install Git for version control management

``` brew install git ```

Install Rbenv for Ruby version management

``` brew install rbenv ```

 Add the command eval "$(rbenv init -)" to your ~/.bash_profile file to make rbenv load automatically when you open up the Terminal.

Install the Ruby langage using Rbenv, and set default version

``` rbenv install 3.1.3
    rbenv global 3.1.3
```

Install Rails web framework

``` gem install rails -v '7.0.4.2' ```

## Install and Run Server Application

* From your terminal, navigate to the root directory for your development projects

``` cd /Users/<username>/Projects ```

* Clone this Github repository into your projects directory

``` git clone https://github.com/soundobjects-xyz/server.git ```

* Change directories to the cloned repository

``` cd server ```

* Create the local development / test databases, and seed the database with default data

``` rails db:create
    rails db:migrate
    rails db:seed
```

* Start the rails server in a terminal

``` rails s ```

* Open a browser and access one of the sample endpoints:

[Sounds Endpoint (JSON)](http://localhost:3000/api/v1/sounds)

If the server is working, you should receive a stream of JSON data with the 10 sample JSON sounds from your local database.

## Contributors

[Greg Richardson](https://github.com/jgrichardson)
[Jason Shannon](https://github.com)

## License

This project is released under the MIT license:

[MIT License](https://opensource.org/licenses/MIT)





