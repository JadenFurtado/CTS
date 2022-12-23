# CTS

Capture the signal!

The work in this repo is heavily influenced by work done <a href="https://github.com/capturethesignal/cts-backend">here</a>, by <a href="https://github.com/capturethesignal/">Capture the Signal (CTS)</a>

I have used my own docker container for the purposes of compiling and running the GRC files, however, the idea behind it remains largely the same as done in the CTS repos

## Usage:

Build the base container using the command:

```
docker build -t capturethesignal .
```

Add the GRC files required for generating the challenge RoIP signals in the Challenge_<challenge id> folder.
Make necessary configuration changes to the docker-compose file. 

* To launch all challenges, Run: 

```
docker-compose up
```

* To launch a selected challenge, Run:

```
docker-compose up Challenge_<challenge_id>
```

Note: While the work done previously works fine, it breaks for newer versions of GNU Radio as they have shifted from XML to YAML :) Also, I had a hard time making changes to the challenges and so, decided to go ahead and build this based of that.