---
title: Channel Configuration
date: Last Modified 
permalink: squeryl_setup/setup/channelConfig.html
eleventyNavigation:
  key: channelConfig
  order: 6
  title: Channel Configuration
---

Squeryl works best when it it has been properly configured in a Slack channel. There are three things you can configure to make Squeryl work better for you:
- Connecting Google Search Console
- Connecting Google Business Profiles
- Subscribing to Automated Reports

To configure one of these for a channel, type the relevant command into Slack and follow the prompts.

Let’s see what each options does and learn how to use it:

#### Connect Search Console

This allows you to connect Google Search Console properties to a specific Slack channel. This allows you to use Squeryl to manipulate and pull information from GSC into the channel. Make sure to select all the properties you need for that channel, and remember information safety steps.

Type this command in Slack to add GSC properties to a channel:

```
/search-console add
```

This command will let you list the GSC properties connected to the current channel:

```
/search-console list
```

And lastly, this command lets you reset the current channel and remove all properties connected to it.

```
/search-console clear
```

Squeryl securely stores user data in an S3 bucket, and doesn’t access it for
any other purpose. Squeryl also doesn’t store any user data on the server.

![Squeryl Config - Connecting Google](/images/connectwithgsc.png)

#### Connect Google Business Profile

This allows you to connect Google Business Profile locations to a specific Slack channel. This allows you to use Squeryl to manipulate and pull information from Google Business into the channel. Make sure to select all the locations you need for that channel, and remember information safety steps.

Type this command in Slack to add Google Business locations to the current channel:

```
/google-business add
```

Use this command to list the Google Business locations connected to the current channel:

```
/google-business list
```

And lastly, this command lets you remove the locations connected to the current channel:

```
/google-business clear
```

Squeryl securely stores user data in an S3 bucket, and doesn’t access it for
any other purpose. Squeryl also doesn’t store any user data on the server.

![Squeryl Config - Connecting Google](/images/connectwithgmb.png)

#### Automated Reports

So now that you've added Search Console Properties and Google Business Locations, you can receive automated reports based on your Search Console and Google Business data. Right from the comfort of your Slack workspace.

This is a great way to keep your team up to date with the latest information. The reports will be sent to the main thread of the channel it is set up in. For example, if you want a weekly report sent to the #marketing channel, you would set it up in the #marketing channel.

Type this in the channel to set up automated reports:

```
/reporting
```

Then follow the prompts to choose what types of reports you'd like the channel to receive.

![Squeryl Config - Automated Reports](/images/automatedreports.png)

#### Index Monitoring

