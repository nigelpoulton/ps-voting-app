Example Voting App
=========

Originally forked from [here](dockersamples/example-voting-app).

Updated cosmetically for Pluralsight courses.

Relates to two Docker images (v1 and v2) [here](https://hub.docker.com/repository/docker/nigelpoulton/tu-demo)

Architecture
-----

![Architecture diagram](architecture.png)

* A Python webapp which lets you vote between two options
* A Redis queue which collects new votes
* A .NET worker which consumes votes and stores them in…
* A Postgres database backed by a Docker volume
* A Node.js webapp which shows the results of the voting in real time

