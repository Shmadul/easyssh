# easyssh
Auto Enter SSH Password Using ~/.ssh/config
Example ~/.ssh/config:
Host nickname
User root 
#Password alpine
HostName localhost
Port 2222
#To Prevent Man in the Middle Attacks from localhost add this to ~/.ssh/config
StrictHostKeyChecking no
UserKnownHostsFile=/dev/null
#Once you've added ^ to ~/.ssh/config, and ran source ~/.bash_profile
#Run ssh nickname and it will automatically login
