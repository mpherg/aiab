# Atlassian In A Box (aiab)

Run JIRA software and Bitbucket Server with a single command!

    docker-compose up

Access JIRA at `http://localhost:8080`, and Bitbucket Server at
`http://localhost:7990`. You can even git fetch/push using SSH at
localhost:7999.

## Data Volumes

JIRA data will be stored in a data container called "jira-data", and
Bitbucket Server data will be stored in a data container called
"bitbucket-data".

## Stuff still to do

- Add Confluence
- Figure out bi-directional data container linking (you can sort of make
this work by linking Bitbucket Server to JIRA using http://jira:8080, and
JIRA to Bitbucket Server using http://bitbucket:7990, but it doesn't work
very well because the display name is localhost...
