Created an image that contains the Ruby on Rails environment ready with Helsinki time zone.

Just create a new project with rails new <project-name> or copy an existing one and start the server with

rails s -b 0.0.0.0

The "b 0.0.0.0" was required because Docker maps to the address 0.0.0.0 by default:
docker port <container>
3000/tcp -> 0.0.0.0:3000