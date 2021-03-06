# Ruby on Rails Tutorial: sample application

This is the sample application for the [*Ruby on Rails Tutorial*](http://railstutorial.org/) by [Michael Hartl](http://michaelhartl.com/)

This sample application is also live on [Heroku](http://heroku.com/) at http://stormy-waters-9927.herokuapp.com/

It requires PostgreSQL and needs a functioning local Postgres install. See [how to install Postgres locally](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

Once Postgres is setup, run `rake db:setup` and `rake db:migrate`.

Launch the `rails server` and you're good to go. 

If Rails complains  with `could not connect to server: No such file or directory Is the server running locally and accepting connections on Unix domain socket "/var/pgsql_socket/.s.PGSQL.5432"?`
Then you need to create a symlink to the socket file with `sudo mkdir /var/pgsql_socket/ && sudo ln -s /private/tmp/.s.PGSQL.5432 /var/pgsql_socket`.