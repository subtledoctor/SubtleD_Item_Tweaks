# extra_kits

For BG2, BGEE, SoD, BG2EE, IWDEE

This does nothing except add an extra kit into your game.  It is a fighter kit, but it will not appear in any kit menus.

You can modify extra_kits/num_kits.ini.  If you set the value to >1, then the mod will install more than one kit into your game.  It can be as many as you want.

One use for this is, if you want to play a character with a mod kit from BGEE->BG2EE, and you don't use EET.  Install all your mods up until the first kit mod in both games; then look at kitlist.2da and not the difference in the number of rows in each kitlist table.  Install this mod into the game with fewer rows, and the .ini value set to the difference.  Then install all your kit mods in the same order on both games.  Now all player-selectable kits will occupy the same places in kitlist.2da, kit.ids, etc. If you play a character in one game, export the character, and import him/her into the other game, their mod kit will show up the same in both games.

Another use for this mod: if perchance you install an arcane caster kit and it gets the kitids value of 0x4040 or 0x4080, then the game will force that kit to be an Abjurer or Conjurer, respectively.  If you keep tabs on which kits get installed in your game and the last kit was 0x4039 or 0x4079, then install one dummy kit from this mod to occupy the 0x4040 or 0x4080 spot.  Now you can install the next kit  as 0x4041/0x4081, and you will avoid this annoying engine quirk.