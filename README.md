

### A highly customizable plugin to add Scoreboards on your Minecraft Bedrock Server.

### Features:

 - This plugin adds **scoreboard** to your server.
 - Completely **Event Driven**!! Good bye tasks!
 - Everything is customizable.
 - Easy and simple API for developers to use and integrate ScoreHud.
 - You can find some basic tags via 
 
### How to setup?

 - Put the plugin in your plugins folder.
 - Start and then stop the server.
 - Edit the `config.yml` and `scorehud.yml` to suit your needs.
 - Restart and enjoy.
 
### Version 6.0 Update:

> The main goal of version 6.0 update was to remove ScoreHud dependency pocketmine tasks. So that was achieved by making
> ScoreHud **event driven**! <br />

**Q: But what exactly does event driven mean? And what are its benefits?** <br />
A: Well, its simple, instead of using **tasks** to update values on scoreboard every 20 or so ticks even when there was **no 
update**, ScoreHud now **listens for events** that are fired by the plugin which implements ScoreHud. In doing so, the scoreboard 
is **only updated when there is an actual update** and not the other way round. Although not tested but this should **improve 
ScoreHud's performance**.<br />

**Addon support was removed** with version 6.0 update. Reason being that it was no longer feasible and users had reported addons 
not working on different systems either due to hosting problem or some other reasons. Removing addons and listening to events 
instead should now **work on almost all systems**.<br />

ScoreHud using events is in the **benefit of plugin developers and the end-user** as well. Users no longer will need to download 
and place addons in separate folder. And plugin developers will no longer need to make a separate addon for ScoreHud. They 
can just integrate ScoreHud directly into their plugin and fire events to update their tags
