# Hubot

Hubot is a chat bot, modeled after GitHub's Campfire bot, hubot. He's pretty
cool. He's [extendable with scripts](http://hubot.github.com/docs/#scripts) and can work on [many
different chat services](https://hubot.github.com/docs/adapters/).

This repository provides a library that's distributed by `npm` that you
use for building your own bots.  See the [documentation](http://hubot.github.com/docs)
for details on getting up and running with your very own robot friend.

In most cases, you'll probably never have to hack on this repo directly if you
are building your own bot. But if you do, check out [CONTRIBUTING.md](CONTRIBUTING.md)

If you'd like to chat, drop by [#hubot](http://webchat.freenode.net/?channels=#hubot) on FreeNode IRC.

## License

See the [LICENSE](LICENSE.md) file for license rights and limitations (MIT).

## Deploy

Install Elastic Beanstalk CLI

```
brew install awsebcli
```


Setup Elastic Beanstalk

```
eb init
```

Select region us-east-1 and hubot. Example:

```
jharris:hubot JoshuaHarris$ eb init

Select a default region
1) us-east-1 : US East (N. Virginia)
2) us-west-1 : US West (N. California)
3) us-west-2 : US West (Oregon)
4) eu-west-1 : EU (Ireland)
5) eu-central-1 : EU (Frankfurt)
6) ap-southeast-1 : Asia Pacific (Singapore)
7) ap-southeast-2 : Asia Pacific (Sydney)
8) ap-northeast-1 : Asia Pacific (Tokyo)
9) sa-east-1 : South America (Sao Paulo)
10) cn-north-1 : China (Beijing)
(default is 3): 1
```

### Deploy

```
eb deploy
```

eb deploy will start of new deployment of hubot to prod environment

## Plugins

Plugins are installed in the **scripts** folder.

### hubot-newrelic2

Targeted Victory's fork of hubot-newrelic2 (https://github.com/targetedvictory/hubot-newrelic2)
is installed with support for additional metrics and multiple accounts.  See the
readme at that repository for detailed usage and configuration information.
