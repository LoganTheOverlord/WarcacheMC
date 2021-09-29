# Choosing your permissions plugin (JUST USE LUCKPERMS)
Head to luckperms.net and download latest luckperms for your server version in "Bukkit" section.

# Adding permissions to default group
It's as easy as running "/lp group default permission set %permission%"

# Removing/Denying permissions to default group
To do this, we use "/lp group default permission set %permission% false". If you want to otherwise enable it, change "false" to "true"
  
# Creating a new group
-> "lp creategroup <groupname>
  
# Inheriting default permissions to created group
To do this, we use "lp group %group% parent set default". This will work with any group instead of default, and vice versa. This means that this group has
it's own permissions, as well as default permissions.
  
# TIMED RANKS, YES!
Now, this is kinda funny. I figured this out too late, but let's share it!
Use "lp user %user% parent addtemp %group% 1d". This will add a permission group to player for limited time. Use 1d, 1m, 1s, etc. (or 7d, 14d, 30d, etc)
  
# SETTING/GIVING RANKS
Use "lp user %user% parent set %group_"
This will clear all parent groups and will set it to desired one.
  
# Removing permissions
use "lp group %group% permission unset %perm%"
  
# Setting display name of group (for use with %vault_rank% placeholder to display tag)
use "lp group %group% setdisplayname %name%"
  
# USAGE
Please note that set and unset commands in scope of permissions, parents, etc. work both for users and groups.
