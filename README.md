# Alfred Asana

Just like the extension this was completely copied from, it is dead simple. It just maps `asana ...`
to calling the [Asana Command-Line Client](https://github.com/tmac721/asana-client) command (`asana`),
passing all the arguments through.

## Installation

[Download](https://github.com/jadb/alfred-asana/blob/master/Asana.alfredextension?raw=true),
then double click the `Asana.alfredextension` file.

It's compatible with the [Extensions Updater](http://jdfwarrior.tumblr.com/updater) extension,
so no need to check back for updates.

Keep in mind that you will need to have the `asana` command installed for it to work.

        $ gem install asana-client

## Usage

While you can technically call any task command, both the native Mac OS Notifications
and Growl don't really show listing results properly.

Adding and completing tasks (get them out of your head and back to focus) is the biggest reason
for writing this.

Thankfully, though, Asana CLI Client lets you key of task id's or unique substrings, so you
can actually work reasonably well blind to do other things:

        $ asana workspace do something due tomorrow
        $ asana workspace/project do something @someone
        $ asana finish 12345

One nice thing is that Alfred also has a command which opens a terminal (by
default mapped to `>`) so entering bigger commands can be done just by prefixing
it with that.

        > asana workspace/project

See more about how it all works [here](https://github.com/tmac721/asana-client/blob/master/README.markdown).

## Credits

http://serialized.net/2012/09/a-simple-taskwarrior-alfred-plugin/
