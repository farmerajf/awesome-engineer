# Awesome engineer
A curated list of software engineering tips and tools

## Git

### Interactive rebase
Interactive Rebase is the Swiss Army Knife of tools in Git: it allows you to do and change almost anything.

The first step is to identify the last "good" commit and provide its hash to the rebase command:
`$ git rebase -i -p 0ad14fa5`

Your editor will open, requesting you to mark all the commits you want to change with the "edit" keyword.
![interactive-rebase](images/01-interactive-rebase.png)

Git will now walk you through each commit, giving you the chance to mold it as you desire:
```
Stopped at 5772b4bf2... Add images to about page
You can amend the commit now, with

    git commit --amend

Once you are satisfied with your changes, run

    git rebase --continue
``` 

<sub>Source: https://www.git-tower.com/learn/git/faq/change-author-name-email/</sub>


## Github

#### Github SSH setup
- Create the directory `~/.ssh`
- Copy and paste your PRIVATE SSH key into a file called `~/ssh/id_rsa`


## Postgres

## Docker container
Create a Postgres DB in a Docker container using the following:
`$ docker run --name <container-name> -e POSTGRES_PASSWORD=<password> -d postgres`

This command uses the official [Postgres Docker image](https://hub.docker.com/_/postgres). Refer to the [Docker image page](https://hub.docker.com/_/postgres) for information on how to change defaults.
The default database name and user is `postgres`.

<sub>Source: https://hub.docker.com/_/postgres</sub>
