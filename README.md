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
# Spigot.yml
Here, set view-distance again to 2.
Also set:
- max-entity-collisions: 2
- arrow-despawn-rate: 120
- mob-spawn-range: 2
- hopper-amount: 1
- entity-activation-range:
      animals: 16
      monsters: 20
      raiders: 28
      misc: 8
      water: 8
      villagers: 16
      flying-monsters: 32
      villagers-work-immunity-after: 100
      villagers-work-immunity-for: 20
      villagers-active-for-panic: true
      tick-inactive-villagers: true
      wake-up-inactive:
        animals-max-per-tick: 4
        animals-every: 1200
        animals-for: 100
        monsters-max-per-tick: 8
        monsters-every: 400
        monsters-for: 100
        villagers-max-per-tick: 4
        villagers-every: 600
        villagers-for: 100
        flying-monsters-max-per-tick: 8
        flying-monsters-every: 200
        flying-monsters-for: 100
- ticks-per:
      hopper-transfer: 20
      hopper-check: 20
- entity-tracking-range:
      players: 48
      animals: 20
      monsters: 20
      misc: 20
      other: 20
 -  max-tnt-per-tick: 1
    enable-zombie-pigmen-portal-spawns: true
    item-despawn-rate: 6000
    view-distance: 2
    wither-spawn-sound-radius: 0
    arrow-despawn-rate: 122
    trident-despawn-rate: 122
    hanging-tick-frequency: 100
    zombie-aggressive-towards-villager: true
    nerf-spawner-mobs: false
    mob-spawn-range: 2
    end-portal-sound-radius: 128
    max-entity-collisions: 2
    
Those are optimized settings for spigot server! It should increase your performance, however, we need Paper for it to work!

