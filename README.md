# docker-ssh-automator

Let's automate to get in a docker container to make it easier by selecting its name.

**Step 1** First create a bin directory at your user folder on your host machine (if not exists) and then export path to your `.bashrc`. Simply you can copy the below line and run it on your terminal:

```ruby
cd ~;mkdir -p bin;echo "export PATH=$PATH:$HOME/bin" >> .bashrc
```
Of course you can do it manually too.

**Step 2** Copy `docker-ssh` file to your `~/bin` folder.

**Step 3** Make the file executable by and then source the `.bashrc` file:

```ruby
chmod a+x ~/bin/docker-ssh
source ~/.bashrc
```

**Done!**

Now you can easily call 

```ruby
docker-ssh
```

..from anywhere you like. It will list the container names and ask you to select which one you want to get in by `/bin/bash` entrypoint.

![Preview](https://image.ibb.co/kpS6nG/preview.png)

Please note Docker should be running in your system and you should have running containers to list them :)

Enjoy...
