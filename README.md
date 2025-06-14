# 15.x-with-8.60

Hi,

I've downgraded the 15.x assets to 8.60 DAT and SPR using SpiderClientConverter. I've added all original 8.60 outfits, items, and effects.
This gives you a complete 8.60 client with content from versions up to 15.x.
I converted every single item from 8.60 by hand from asynchronous to synchronous. This means idle animations for outfits now work perfect and we don't have any bugs or visual glitches in the animation
Note: We've also imported all outfits from version 9.83 (up to ID 537), so you now have 3-frame animations and full mount support (looks like 8.60). If you prefer the original 8 frame animation for outfits you can change it by urself without problems :D

OTCv8 Features that need to be enabled in order to use this:
    
    g_game.enableFeature(GameEnhancedAnimations)
    g_game.enableFeature(GameIdleAnimations)
    g_game.enableFeature(GamePlayerMounts)
    g_game.enableFeature(GameSpritesU32)

NOTE: To avoid problems with map saving make sure to change in your rme files under data/clients.xml

from
# <otb client="8.60" version="3" id="20"/>
to
# <otb client="8.60" version="3" id="64"/>