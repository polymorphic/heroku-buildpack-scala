# This is a fork of [Heroku Scala Buildpack](https://github.com/heroku/heroku-buildpack-scala)

The modified Scala Buildpack provides support for
[sbt multi project builds](http://www.scala-sbt.org/0.13/tutorial/Multi-Project.html). To
use an entry point in a project other than the default (e.g., for
project foo you'd use ```sbt foo/compile```) inject the name of the
project via the environment variable ```SBT_PROJECT``` (leave it unset
for the default behavior).
