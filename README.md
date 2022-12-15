Learning how to make a helpful bot

### Setup instructions
* install Go, git, a text editor

### how to git
```
eval "$(ssh-agent -s)"        // for permissions
git add <filename>
git commit -m "update readme"
git push

#### nice commands
* `git log`: see the history
* `git status`: see the current status of your changes
* `git diff`: see the diff of your changes

### setup go
* `go mod init`


# Development
### Build and run
* `git pull` to grab the latest
* run `go build` to build
* run `./voice_receive -t <secret-bot-token> -g 534260764182183936 -c  607312321156612137`
  * where `-g` is the guild ID of your server, and `-c` is the channelId
  * secret bot token is the token of the bot itself

# Refs
### ref: adding voice_receive
* copy require stuff in `go.mod`
* run `go mod tidy`
* run `go build`

### refs
* https://github.com/bwmarrin/discordgo
* https://github.com/bwmarrin/discordgo/tree/master/examples/voice_receive
* https://gabrieltanner.org/blog/dicord-music-bot/