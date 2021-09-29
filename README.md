# WarcacheMC

Why is Warcache interested in Minecraft development?
- We want to contribute to wellbeing of every modern Minecraft server, and modpack.
- Thus, we provide configurations, which will extend your abilities to have greater performance, more players, less CPU and RAM usage, etc.
- We are also interested in modpacks! (See Project: Immersion)
- We learn a lot of new things in process. And what else would we want? <3

# Why is this important?

We believe that if we share our knowledge, we give more people more opportunities to not only create better servers, but mainly hope to educate people in their way for quality servers. It's easy to set-up server, however, quality content is usually hidden behind years of work.
With this, we hope to share the best of our knowledge to make servers great again.

# Configuring Spigot for Performance

There are many things you can do to increase performance of your server. We'll talk about every configuration file of PaperMC and in respect of that, provide you with optimization tips.
# Server.properties
There is not as much to be done, however, for the first thing, I want you to set view-distance to value =2
This will trick server into ticking only 2 chunks in range. I'll explain why we do this later on.
# Spigot.yml, Paper.yml, Bukkit.yml
We have created optimized settings for each of these, including custom messages. You can change these. Just drag&drop upload it to your server to see results.
In regards to view-distance trick, we have set no-tick-view-distance in paper.yml, which means you will see 7 chunks render, but only 2 chunks will be ticked.

