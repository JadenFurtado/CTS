# CTS

Capture the signal!

The work in this repo is heavily influenced by work done <a href="https://github.com/capturethesignal/cts-backend">here</a>, by Capture the Signal (CTS)

I have used my own docker container for the purposes of compiling and running the GRC files, however, the idea behind it remains largely the same as done in the CTS repos

## Usage:

Add the GRC files required for generating the challenge RoIP signals in the Challenge_<challenge id> folder.
Make necessary configuration changes to the docker compose file.

To launch all challenges, Run: 

```
docker-compose up
```

To launch a selected challenge, Run:

```
docker-compose up Challenge_<challenge_id>
```
