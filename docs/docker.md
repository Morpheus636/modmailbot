# Docker Setup
This is intended only for advanced users who already have experience using Docker.
If you are looking for traditional deployment, look at [Starting the bot](starting-the-bot.md)

1. Install Docker on your host machine.

2. Configure ModMail
  - Follow the instructions in [Setting up the bot](setup.md) to go through prerequisites and config!

3. Pull the `morpheus636/modmailbot` image from DockerHub

4. Deploy your ModMail container
  - Make sure you populate the following volumes:
    - `config.ini`: Mount your config.ini file from a location on your host machine to this volume.
    - `db/` : Mount a directory on your host machine containing your `data.sqlite` file to this volume,
    assuming youre using sqlite.