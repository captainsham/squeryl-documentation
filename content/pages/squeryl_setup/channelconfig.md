title: Channel Configuration
date: Last Modified 
permalink: squeryl_setup/setup/channelConfig.html
eleventyNavigation:
  key: channelConfig
  order: 6
  title: Channel Configuration
---

You can configure different options in Squeryl by saying @ Squeryl config and following the relevant prompts.

This will bring up a conversational interface where you can configure a couple of different options.

![Squeryl Config](/images/config.png)


Let’s go through what each of these commands do:

#### Connect Search Console

This allows you to connect GSC to the specific channel. This allows you to use Squeryl to manipulate and pull information from GSC into the channel. Make sure to select all the properties you need for that channel, and remember information safety steps.

Squeryl securely stores user data in an S3 bucket, and doesn’t access it for
any other purpose. Squeryl also doesn’t store any user data on the server.

![Squeryl Config - Connecting Google](/images/connectwithgoogle.png)

#### Automated Reports

This allows you to set up automated reports to be sent to the channel. This is a great way to keep your team up to date with the latest information. You can set up a report to be sent daily, weekly, or monthly. The report will be sent to the main thread of the channel it is set up in. For example, if you want a weekly report sent to the #marketing channel, you would set it up in the #marketing channel.

![Squeryl Config - Automated Reports](/images/automatedreports.png)

#### Index Monitoring

