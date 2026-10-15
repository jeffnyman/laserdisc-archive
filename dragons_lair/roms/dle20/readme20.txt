DRAGON'S LAIR ENHANCEMENT ROM SET VERSION 2.0 · September 15, 2002
Dave Hallock · dave@dragons-lair-project.com
Jeff Kulczycki · jeffkul@dragons-lair-project.com

These ROMs contain radical functional changes that require the following text.
This complete document must accompany all distribution of these ROMs.
Mandatory information for proper installation and operation follows.

INTRODUCTION
This ROM set has been created to enhance the gameplay of Cinematronics' 1983 arcade version of Dragon's Lair.  Logical reconstruction to game organization and presentation has been implemented, and the result is what is believed to be the first and only Dragon's Lair game program that plays the game the way it was intended to be played while it was being designed/animated.  This ROM set also optionally makes playable the prototype animation newly recorded at the end of the Dragon's Lair Limited Edition Laser Disc that was pressed in 2002.

ROMS
DLE 2.0 occupies 4 type 2764 EPROMs or compatible.  There is one set of DLE 2.0.  It works with any working Cinematronics DL game using any laser disc player.  The creation of different ROM sets optimized for different laser disc players was not necessary.  These ROMs' internet home is www.dragons-lair-project.com/tech/enhancements/dle.asp  Check there to see if any updates exist.

VERSION
DLE version 2.0 contains the following changes from DLE 1.1.
· Scene presentation has been redesigned to better match the animators' original game design theory.
· A DIP switch option accesses the prototype animation on the Dragon's Lair Limited Edition Laser Disc.
· There are no game difficulty options of any kind.  The prototype game data has replaced the hard difficulty game data.
· There are several new DIP switch options and enhancements to previous options (described below).
· Game scoring has been restructured and charted.  Scores increment in the display at the moment creatures are destroyed.
· Auto-optimization for the original disc players has been implemented.
· Various small updates have been made to the gameplay data.

SETTINGS
New DIP switch features include:
· 1 coin per credit & 4 coins per credit game pricing options
· 1 or 2 coin pay-as-you-go pricing options
· standard and prototype game play modes
· exclusion of narrator voice from attract mode audio

Note: The DIP switches on the main PCB are numbered from 0-7, not 1-8.

DLE 2.0 DIP switch settings chart:

···············································································
A. Attract Mode Sound
     Always on ································ B0=ON,  B1=ON
     Plays every 8th time ····················· B0=OFF, B1=ON
     Always off ······························· B1=OFF
     Attract sound includes narrator voice ···· B4=ON  (ORIGINAL FOR STANDARD)
     Narrator voice muted* ···················· B4=OFF (ORIGINAL FOR PROTOTYPE)

B. Number of Coins Required for One Credit
     1 ········································ A0=OFF, A1=OFF, A4=ON
     2 ········································ A0=ON,  A1=ON,  A4=ON
     3 ········································ A0=OFF, A1=ON,  A4=ON
     4 ········································ A0=ON,  A1=OFF, A4=ON
     2 credits at all times/free play ········· A4=OFF

C. Number of Dirks Per Credit
     3 ········································ A5=ON,  B2=ON
     5 ········································ A5=OFF, B2=ON
     Unlimited Dirks for testing purposes ····· B2=OFF

D. Playtest and Diagnostics
     Normal operation ························· A3=ON,  A7=ON
     Playtest for engineering use ············· A3=OFF
     To run diagnostics, set A7 to ON, and
       power up the game.  After you hear two
       beeps, turn A7 to OFF.  Turn A7 back to
       ON to end diagnostics. ················· A7=first ON, then OFF

E. Game Mode
     Standard ································· B7=OFF
     Prototype**······························· B7=ON

F. Pay-As-You-Go Play Options
     Pay-as-you-go disabled.  The game ends
       when won. ······························ A6=ON,  B5=ON
     Pay-as-you-go disabled.  The game starts
       again from the beginning when won. ····· A6=ON,  B5=OFF
     The player must deposit 1 or 2 coins
       (depending on A2) to continue playing
       once, after 2/3 of the game is finished.
       The game ends when won. ················ A6=OFF, B5=ON,  A4=ON
     The player must deposit 1 or 2 coins
       (depending on A2) to continue playing
       two times during the game, and may
       deposit more coin(s) to continue again
       from the beginning after the game is
       won. ··································· A6=OFF, B5=OFF, A4=ON
     The player receives one additional Dirk
       after depositing coin(s) to continue
       (during the first game only). ·········· B6=ON
     No extra Dirks are awarded. ·············· B6=OFF
     The price to continue is 1 coin. ········· A2=OFF
     The price to continue is 2 coins. ········ A2=ON

G. Disc Player Model Selection***
     Pioneer PR-7820 ·························· B3=ON
     Pioneer LD-V1000 ························· B3=OFF
···············································································

*On the Dragon's Lair Limited Edition Laser Disc, the narrator's voice is newly dubbed over the prototype attract mode audio.  The original state of the prototype attract mode is without the narrator's voice.  DIP switch B4 allows user selection either way for both game modes.

**The prototype game mode setting requires the Dragon's Lair Limited Edition Laser Disc pressed in 2002.  The controls for the prototype game differ, as explained later.  Note:  The PR-7820 disc player is not compatible with the limited edition disc.

***DLE 2.0 auto-optimizes its video playback to the disc player selected by DIP switch B3.  When B3=ON, video segments will stop playing 3 frames sooner than when B3=OFF.  If you are using modern disc player conversion hardware, you may be able to use B3 to manipulate the video play time on your system.  If scenes end too early, set B3=OFF to extend the video play time.  If scenes play too long, set B3=ON to shorten the video play time.  (And of course, your conversion hardware must be compatible with the setting of B3.)

SCORE CHART
DLE 2.0 has a new and structured scoring scheme:

···············································································
Making a correct move:
· during the 1st Castle Section ·   684
· during the 2nd Castle Section · 1,173
· during the Caverns Adventure  · 1,679
· in the Dragon's Lair          · 2,000

Killing enemies:
Snake · 1,750
Bat · 1,750
Parry a weapon · 1,750
Cyclops Worm Creature · 2,000
Skull · 2,250
Tentacle · 2,500
Skeletal Hand · 3,000
Spider · 3,000
Giddy Goon · 3,500
Slime Monster · 4,000
Crypt Creep · 5,000
Smithee · 7,000
Giant Bat · 10,000
Cauldron Wizard · 12,000
Grim Reaper · 15,000
Lizard King · 15,000
Robot Knight · 17,500
Mudmen · 17,500
Black Knight · 20,000
Dragon · 25,000
···············································································

ENHANCEMENTS (BASIC)
A standard game of DLE 2.0 can basically be described as DLE 1.x with scene resequencing.  This section is a condensed description of the basic and well-known DLE features.  If you are not familiar with any previous version of DLE, please read this section.  Otherwise, you may wish to skip this review and jump ahead to the "NEW" enhancements section.

All animation segments recorded on the laser disc are now accessible by the game program.  All of the scenes and death scenes that were originally never used are now part of the game.  All times have been lengthened so that all scenes will play on-screen until their very end.  All main scenes will begin playing from their starting points on the laser disc, and will play through in their entireties.

Almost all times have been adjusted so that if you make no move, you will no longer see Dirk make the correct move on-screen before he dies.

Immediately before each main scene on the disc is a "resurrection" scene where Dirk is brought back to life from a skeleton.  Resurrections now play smoothly into the beginning of the main scene without a disc player search.

During a 2-player game, each player's game now starts with the opening shot of the castle.

Drawbridge : The drawbridge scene has been added to the start of the game.  The small yellow room with 3 doors and falling rocks is played as part of the drawbridge scene.

Tentacles · halberd : The last move must be made while the door is open.

Mist room · snakes : The third move is always now required, and doing nothing will cause death.

Bedroom · filling wall : The death scenes' appearances better correspond to the player's input (or lack thereof).

Giddy Goons : There is now more than one successful way to deal with the first giddy goon.  The last move is always now required, and doing nothing will cause death.  There is now more than one successful way to deal with the last remaining giddy goons.

Flattening stairs · Cyclops Worm Creatures : There is now more than one successful way to deal with the Cyclops Worms.

Lizard King · pot of gold : There is now more than one successful first move to this scene.  The final battle with the Lizard King requires new joystick moves to match Dirk's actions.

Grim Reaper · spinning socker boppers : This scene now plays from the beginning, which more than doubles the time Dirk may remain in front of the socker boppers.  The original program's timing has always been such that the first move should be made immediately after both boppers swing across the center path together at the same time.  This timing structure has been preserved, and the full length of the animation allows 7 chances to successfully make the first move.

Mausoleum · Crypt Creeps : The original program occasionally played 2 death scenes if you lost your last life at the bouncing skulls.  This has been corrected.

Pool · spider : There is now more than one successful way to deal with the spider.

Chapel · Robot Knight : All incorrect joystick moves will now kill Dirk.

Elevator floor (a.k.a. falling platform) : Dirk is now always seen successfully jumping off of the platform in the same direction that you moved the joystick.

Giant Bat : There is now more than one successful way to deal with the first bat attack.  After killing the giant bat, a move is required.

Catwalk · bats : The original program suffered a timing error if your second move was left.  The timing has been corrected.

Rolling balls : You must wait a little longer for the colored balls to clear your path before moving.

Mudmen : The second, fourth, and seventh moves have been changed to correctly match Dirk's actions.

Dragon's Lair : The original program gives a buzz sound for many incorrect moves that can made in the lair.  Most wrong moves now result in death.  A new move is required to position Dirk for the final kill.  The post-game still frame of Dirk & Daphne is no longer jittery as it always was on a LD-V1000 player.

ENHANCEMENTS (NEW)
New to DLE 2.0, the scenes' playing order has been restructured.  The scenes have been segregated into castle sections, consistent with the pay-as-you-go text messages on the laser disc.

The Castle Sections
· The Drawbridge
· Castle Section 1 · All of the small, short, easy, one-roomed scenes are played first.
· Castle Section 2 · The longer, harder, and reversible scenes are played next.
· The Elevator Floor · The falling platform delivers Dirk to the mysterious caverns below the castle.
· The Caverns Adventure · This section contains all of the cavernous themed scenes.
· The Dragon's Lair

Whenever you lose a life, the scene that you died on will appear once again when you've reached the end of the castle section it is in.  If you die on the same scene a second time, then the scene will be skipped (permanently) and the game will continue.  (Exception: if you die on the drawbridge twice, you'll advance into the yellow room.  Any time you die in the yellow room, it will be permanently skipped.  If you die in the dragon's lair, it will repeat indefinitely.)

You are no longer required to complete both orientations of the reversible scenes during the same game.  One orientation of each reversible scene will be randomly selected.  If you die on a reversible scene, then when it appears the second time, it's still possible that it could be reversed from the first time you encountered it.

Within castle sections 1 & 2, the scenes will appear randomly.  They are selected using the established method of picking them from among groups of 3.  The sequencing of the caverns adventure is determined by the point at which you decide to jump off of the falling platform.  A scene sequencing diagram for DLE 2.0 can be found online at the DLE home page.

Prototype Game Mode
Recorded at the end of the Dragon's Lair Limited Edition Laser Disc is over 8 minutes of test animation that was used in the prototype Dragon's Lair arcade game and then left on the cutting room floor.  These 12 scenes are substantially different, in that there are usually multiple branching opportunities within them, as well as multiple conclusions to half of them.  For users of this disc, the prototype DIP switch setting makes these scenes playable, and swaps them in to replace their standard animation counterparts within the normal game.

The game play controls differ for the prototype mode of DLE 2.0.  Like the prototype arcade game cabinet, this game mode uses the original design concept of an "ACTION" button on the control panel instead of a "sword" button.  The "ACTION" button causes Dirk to use his hands.  Any time that you want Dirk to grab something, use something, or manipulate anything with his hands, you must press "ACTION".  When a monster is present, then generally, the "ACTION" button causes Dirk to draw and use his sword.  The joystick is only for directional movement.  If you try to use the joystick to move Dirk into an object that you want him to handle with his hands, you will only hear a buzz sound, or else you may even lose a life!

Note:  The limited edition disc stretches beyond the standard 30 minute capacity for CAV discs.  If your disc player has trouble accessing some prototype scenes, the player may need cleaned, or it may not be able to handle discs of this length.  At the time of this writing, no industrial disc player models have been identified as being unable to play the whole disc, with the exception of the PR-7820 which is not compatible with the limited edition disc overall.  You can find out more about the limited edition disc and disc player technical assistance at www.dragons-lair-project.com

Attract Mode
The DIP switch option to play the attract mode audio only 1 out of 8 times now plays the audio on the first time after power-up, instead of the 8th time.

If a start button is pressed while the game contains only partial credit, a text message instructing to "deposit more coins" is briefly displayed.

Pay-As-You-Go
This feature has been enhanced.  As before, it requires players to deposit more coins to continue their game when they've reached certain points, but now, the text prompts directly correspond to the various castle sections.  These messages are the foundation of DLE 2.0's new scene sequencing, so give this feature a try just for fun.  P-A-Y-G now always requires a new coin drop when prompted.  Originally, it stole any existing credit that might be in the game, whether you wanted to continue or not.  A player now has more time (30 seconds) to insert coins when prompted.  In free play mode, P-A-Y-G settings are disabled.  The game is free to start and plays through without interruption.

Q & A
Q.  How did you determine how to program the prototype scenes?
A.  Although no official records or software could be provided by the game's creators, much research was done to determine the original plan for how these scenes were designed to play.  We have a handful of articles from 1983 that describe the play of the prototype game and actually reveal some of the moves.  The original prototype gameplay instructions were studied.  The action in each video segment was carefully analyzed, and nothing was assumed or taken for granted or face value.  The coding written on the clapboard images between the video segments generated a sequential pattern which gave insight into the intended progression of each segment and how they should branch.  Finally, in some dire cases, by consensus with consultants, we decided to mix in some of the standard animation into certain prototype scenes in circumstances where there were critical deficiencies in the available prototype footage.  (For example, there is no prototype death scene for the Cyclops Worms under the drawbridge, nor any prototype footage of Dirk choosing the red flask of liquid.)  Given what was available, we feel that DLE 2.0 offers the most respectful yet complete arrangement of this material.

Q.  What if I set DIP switch B7 to prototype mode while using an original DL disc?
A.  Upon booting up, the game would attempt to search for the prototype attract mode, which is recorded beyond the point that the original disc ends.  The disc player would fail this search, and the game would not run.

Q.  In prototype mode, why don't the game play instructions appear during the attract mode?
A.  The on-screen instructions describe the use of the sword button, but the prototype game mode has an action button, so the instructions are not shown.

Q.  I need some help.  What are the moves?
A.  The readme files for all past Enhancement ROM work have revealed all new moves.  This time however, it is too complex to try to describe all of the prototype scenes' branch points in text.  If you are truly stuck, Dave Hallock might be available to help via email.  The forums of www.dragons-lair-project.com may also be of assistance.

Q.  Why did you make it so that you don't play both versions of the reversible scenes?
A.  It is the original game design.  The reason that some scenes were filmed in reverse was to add variety, difficulty and longevity to the game, by making it so that from game to game, certain rooms of the castle would be unpredictable in appearance, and thus not become memorized as quickly.  They were not reversed with the expectation that people would have to play through them twice in an unrealistic manner, and end up memorizing them just as fast as the others.  When animating the game, the goal was for the castle to be a real-world environment, and for the story to present itself rationally with the coherence of a film.  But ultimately in the end, the final editing of this film became the job of the programmers, who were not film editors.  They apparently either lacked continuity skills or didn't see anything inherently wrong with having both versions of the reversible scenes in the same game.  Thus a disservice was done.

Q.  So then why do you play a scene over again if you die on it?  Where's the continuity there?
A.  Where's the continuity of being able to do ·anything· after dying?  The magic of resurrecting includes the magic of having to try the scene one more time.  And, for the purpose of continuity, you'll retry it while still in the same castle section.  Finish the game without dying, and you'll have a perfectly continuous story.

Q.  Why does the free play setting disable pay-as-you-go settings?
A.  There were 5 different ideas offered on how to handle the simultaneous enabling of these two options.  The easiest and most intuitive conclusion was that free play should make the game completely free no matter what, and that the game should never display any "insert coins to continue" messages without really meaning it. 

ACKNOWLEDGEMENTS
Valuable assistance and consultation by Jeff Kinder and Warren Ondras.  Special thanks to Rob DiNapoli's initial work in this area.

DISCLAIMERS
The user is solely responsible for any and all adverse effects resulting from the use or misuse of this ROM data or the EPROMs it is stored on.  The only intended application of these ROMs is to be installed into a Dragon's Lair arcade game and used privately by the game's owner.  You are instructed not to use them in any other capacity.