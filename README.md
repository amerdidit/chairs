###What am I going to install (with chef)?
- ruby 2.2.0 (rbenv)
- rails (latest stable version)
- passenger 5.0.0.rc2
- mysql (user: root | pass: admin)
- nginx 1.7.10

###Ok, What should I do?
```cmd
$ git clone git@github.com:amerdidit/chairs.git chairs
$ cd chairs
$ cd vagrant
$ vagrant up
$ vagrant ssh
# in the VM
$ sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
$ rails new ../starter
$ bundle install --no-deployment; bundle install --deployment
$ bin/rake db:create
$ rails s
```

now 33.33.33.112 in your browser

## whats next:

1. The app should offer a form to enter all necessary information regarding his request (see
questionnaire attached)
2. Integrate an image upload into the form for the user to upload pictures of his room and
existing furniture. He should further be able to upload a floor plan if necessary.
3. On submit the request should be stored in the database.
4. Build a list of flat information, with each entry representing one request, so the interior
designer can view all requests.
5. Each request should have a state field. The available states are “open”, “in progress” and
completed. The interior designer should be able to change the state.
6. Add Email communication to the flat information view, so the interior designer can contact the
requester directly from the app.

