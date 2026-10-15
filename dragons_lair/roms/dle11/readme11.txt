DRAGON'S LAIR ENHANCEMENT ROM SET VERSION 1.1 - February 29, 2000
Dave Hallock - dave@d-l-p.com

Please include all of this text with any distribution of these ROMs.
Mandatory information for proper installation and operation follows.
Thank you!

INTRODUCTION
These ROM sets have been edited to enhance the gameplay of the (North American) arcade version of Dragon's Lair by utilizing the laser disc's full potential.  The methods that the original program employed to shorten scenes and keep gameplay brief have been eliminated.  Some logical reconstruction to game organization and presentation has been implemented, and some new choices and branching during gameplay are possible, all without radical change or dissimulation from the overall original game structure.  Also, a handful of typos in the original data that negatively affected game performance have been discovered and corrected.

ROMS
There are two ROM sets; each set contains four ROMs.  Set DLE11UxP is optimized for use with the PR-7820 laser disc player & rev. A boardset.  Set DLE11UxL is optimized for the LD-V1000 player & rev. C boardset.  The new EPROMs replace the chips at locations U1, U2, U3 and U4.  Socket U5 remains empty.  Dragon's Lair uses type 2764 EPROMs or compatible.  Seek experienced help with installation.
The only difference between the two ROM sets is how values of time are defined.  Different disc player & boardset combinations behave differently.  Each ROM set has been fine-tuned for its hardware configuration specified above; however, both new ROM sets will function with any configuration and play the same game.  If you are using a rev. A boardset with a LD-V1000, or a rev. C boardset with a PR-7820, it is recommended to use the ROM set optimized for your disc player.  If you are using any other newer model of disc player, you should probably use ROM set DLE11UxL, but only trial & error will determine which set works better for you.
For ANY given hardware configuration, ROM set L will play all segments of video for a couple frames longer than ROM set P does.  (If set L causes video to play too long, set P will shorten all play times.)
These ROMs' internet home is www.dragons-lair-project.com/tech/enhancements/dle.asp  Check there to see if any updates exist.

SETTINGS
All new enhancements are contained in the easy difficulty setting.  DIPSWITCH B7 MUST BE SET TO THE OFF POSITION TO ACCESS THE NEW PROGRAM.  Before modification, these new ROMs began as revision F, and the dipswitch settings for revision F apply to these new ROMs.  (Note: Revision F dipswitch settings are NOT printed in any known game manual.  Find them at  www.dragons-lair-project.com/tech/dips/lair_revf.asp )  Select your disc player with switch B3 ON=PR-7820, OFF=LD-V1000.

VERSION
DLE version 1.1 contains the following changes from DLE 1.0.
- All of the game difficulty options found in the revision F dipswitch settings chart are now available.  DLE 1.1 replaces easy difficulty, and the revision F hard difficulties have been functionally restored.  (A hard difficulty version of the DLE program is not planned.)
- The cauldron/slime scene is now lenient with two incorrect moves (details in the list of changes below).
- The Grim Reaper scene will accept an incorrect first move sooner.
- A sequencing issue regarding the bouncing skulls death scene has been resolved (details in the list of changes below).
- Original scoring for the reversed falling platform has been restored.
- Both falling platforms' death scene sequencing has been restructured (details in the list of changes below).
- (LD-V1000-optimized ROM set only):  A few scenes stop playing one frame sooner.

ENHANCEMENTS
The following is a list of the enhancements provided by these ROMs.  Surprises will be revealed in the text.  If you choose to play the game before reading on, keep this in mind... Try new things!  And expect a very few moves that have been changed to correctly match the action in the animation.

LIST OF CHANGES - WARNING: SURPRISES REVEALED
(These differences concern the easy difficulty setting of the original & new ROMs.)

Note:  N=no move,  U=up,  D=down,  L=left,  R=right,  S=sword

Special Note:  The "original program" referred to several times in the following text is the original Dragon's Lair software revision F, not DLE version 1.0.

All animation recorded on the laser disc is now used by the game program.  The only exceptions are:  1. the first few frames of Dirk being killed by the anvil  2. the first several frames of Dirk failing to grab the chain at the end of the underground river  3. the second (duplicate) appearance of the underground river on the disc and all of its associated scenes.  ALL other animation on the disc not listed above is used.
(Death scenes 1 & 2 above are too long to play in their entirety and still have a fluid transition in the video, because these death scenes contain the initial animation footage that must be viewed before you can choose your move.  To avoid continuity errors, they must be shortened.  However, the 2 scenes now play longer than they used to.)

(To reiterate the above:)  All times have been lengthened so that all scenes will play on-screen until their very end.  This means that you will always see the black circle close up after each death scene, and no scene will stop playing too soon.  All main scenes will begin playing from their starting points on the laser disc, and will play through in their entireties.

Almost all times have been adjusted so that if you make no move, you will no longer see Dirk make the correct move on-screen before he dies.  (This means that you now have a little less time to make many moves.)

Immediately before each main scene on the disc is a "resurrection" scene where Dirk is brought back to life from a skeleton.  The original game program played this resurrection, but then the disc player still blacked out the screen to search for the beginning of the main scene.  This search has been eliminated.  All resurrection scenes now play smoothly into the beginning of the main scene.

During a 2-player game, each player's game now starts with the opening shot of the castle.  Originally, the second player's game did not.

Diagnostics
The color test now displays color bars (as promised by the on-screen text) instead of Dirk's skeleton.  However, some Dragon's Lair laser discs do not contain color bars.  Unfortunately, users of these discs will see a black screen.

Attract Mode
The playing instructions display for eight seconds instead of six.

Drawbridge
The drawbridge scene has been added to the start of the game.  You may move U while Dirk first walks on the drawbridge, but this move is not required and does not award score.  It exists to patronize first-time players and to fill the time.  If you move L or R, Dirk will fall off of the drawbridge and die.  The first required move is either S or U.  (You can choose to ward off the moat creatures with S or climb U right away.)  If you choose S, the next move is U.  The next move is R, and then Dirk runs into the castle.  The small yellow room with 3 doors and falling rocks is then played as part of the drawbridge scene.  If you move D or N as the last move, the never-before-used death scene of Dirk being crushed by the rocks will play.  If you die at any point, the scene will start over.  If you die a second time, Dirk will enter the castle automatically, and the scene is skipped.  It will never replay at the end of the game.

Tentacles - bench in middle of floor
Move R for the second move, and Dirk will climb the stairs (and die).  The last move must be made while the door is open.  There is now a shorter death scene where Dirk is not seen drawing his sword before the tentacles wrap around him.

Snakes (red white & black stripes)
The third move (S) is now required; N will cause death.  When the original program played the death scene of the snake crawling on the floor, the disc player performed a search for the last half of the scene.  This death scene now plays smoothly without the search.

Ropes - fire
---normal---
If you grab the first rope after the ledge recedes, the original program's timing required all remaining moves to be made a bit sooner than usual.  This timing has been corrected.
---reversed---
The third and fourth moves now both award score.  The original score was zero for each.
---both normal & reversed---
The last move must now be made slightly sooner than in the original program, so that the corresponding death scene may be played in its entirety with good continuity.

Pool - spider - other deadly stuff
The first move is not accepted until the floor crumbles away.*  The never-before-used death scene of Dirk falling forward into the crevice is now used with the third move.  The fifth move is not accepted until the snakes appear.*  You may choose to move L or R (as appropriate) instead of S to kill the spider.
*prevents premature guessing of the move

Black cauldron - slime - monsters
Moving L for the first move will give a buzz instead of killing you.  Moving R for the third move will give a buzz instead of killing you.

Giddy Goons
The first move may be either S to kill a goon, or R to climb the stairs right away.  The next move after R can no longer be a quick U.  It is S after the goons appear at the top of the stairs.  The last move now awards score and is now required; N will cause death.  You have until Dirk jumps to the top step to make the last move (U or L).  Or, you may choose S when the last goons appear from below, to safely kill an extra goon for more points. 

Flattening stairs - purple monsters - water behind wall with chain
The third move (L) is now required; N will cause death.  The second move may now be L, U, or S.

Grim Reaper - spinning obstacles - thorns
This scene now plays from the beginning, which more than doubles the time Dirk may remain in front of the spinning obstacles.  The original program's timing has always been such that the first move (U) should be made immediately after both spinning obstacles swing across the center path together at the same time.  Enough animation was played to allow this to happen 3 times, giving you 3 chances to move U. (The timing was never based on sound cues or Dirk's movements... Go try it!).  This timing structure has been preserved, and the full length of the animation now allows 7 chances to successfully move U when the obstacles both cross the center path at the same time.*  Move D for the first move, and the thorns will kill Dirk.  If no first move is made, there is a new shorter death scene where Dirk is not seen running toward the spinning obstacles before they hit him, suggesting that he just must have been standing too close.
*The timing for the first move is programmed differently for ROM sets L and P.  If you are not using the original hardware configuration that the ROM set is optimized for, it's possible that the timing for the first move may grow a couple frames inaccurate when you wait for the later chances to make the move.

Wind/hurricane - exploding door - gem - junk flying around
You may move U or R to approach the first door, but this move is not required and does not award score.  It exists to fill the time.

Filling brick wall in the bedroom
Move U in time, and you will hear a beep and be successful.  Move U too late, and you will hear a beep, and Dirk will be crushed in the wall.  Move N or D, and Dirk is killed by poison gas.

Lightning/bolts from hole in ceiling - fire - bench covers exit
When the original program played the death scene of Dirk jumping for the door, the disc player performed a search for the last half of the scene.  This death scene now plays smoothly without the search.

Flying barding* (horse armor)
Making no move for the first or second move now leads to death by fire instead of crashing into the pillar.
*official name per '83 interview with animator Gary Goldman

Robot Knight* (on checkered floor)
---normal---
Incorrect moves now result in death (as in the reversed version) instead of a buzz.
---both normal & reversed---
You may move U or L/R (as appropriate) to jump the gap in the stairs at the end of this scene, but this move is not required and does not award score.  Why?  See the Q&A section below.
*official name per '83 interview with animator Gary Goldman

Crypt Creeps - skulls - claws - ooze
---normal---
The original program played 2 death scenes if you lost your last life by pressing S at the bouncing skulls.  This has been corrected.

Catwalk - bats
Move R for the first move, and Dirk will try to jump to the right (and die).  The original program suffered a timing error if your second move was L.  The timing has been corrected.

Giant bat
Move R right away for the first move, and bats will kill Dirk.  The first move may be either S or L.  After killing the giant bat, a move L is required.

3-level falling platform & small yellow room with 3 doors (stand-alone)
The fourth group of 3 scenes has been eliminated.  Both 3-level falling platforms and the stand-alone yellow room are no longer part of the game.  Why?  See the Q&A section below.

9-level falling platform
---reversed---
If the game ends during this scene, the correct game-over/skeleton scene now plays.  The error that caused the original program to play the start of the underground river instead has been corrected.
---both normal & reversed---
Dirk is now always seen successfully jumping off of the platform in the same direction that you moved the joystick.  The death scene of Dirk nearly missing the jump will always (and only) play when the correct move is made slightly too late.  All other incorrect timing and moves result in the falling death scene.

Lizard King
Along with L, the first move may now be R, but only before the Lizard King jumps to the right side of the screen.  After the final R, the next move is U, and it can no longer be S.  After the U and the following move S, the next move is either D or L and no longer S, D, or N.  The next move S is now required.  The next move is either D or L and no longer S, D or N.  The last move S is now required.  All moves during the final battle now award score.  Why the changes?  See the Q & A section below.

Underground River
You may move U while Dirk is floating underneath the 3 flashing "Ye" signs, but these moves are not required and do not award score.  They exist to patronize first-time players who have been told to follow the flashes, and to fill the time.  Move L for the fourth required move, and Dirk will row through the opening on the left side of the screen and die.

Mud Men
The second move is now L, and U or N will cause death.  The fourth move is now either R or diagonal U&R, and U will cause death.  The seventh move is now either L or diagonal U&L, and U will cause death.  Why the changes?  See the Q & A section below.  Diagonal U&R is now also acceptable for the last move.  The death scene of Dirk shooting up the geyser stream now extends into the next scene of Dirk gasping at the top of the stream.

Black Knight* (on horse)
Move D for the first or second move, and the Black Knight will kill Dirk.
*official name per animators' model sheet

Rolling Balls
You must wait a little longer for the colored balls to clear your path before moving D.  The source of the falling death scene for the last move is changed from the falling platform to the tilting floor.  This is because the camera angle, length, and purplish background color of this death scene seem more appropriate.

Caverns - grate - jagged doors - bridge - geyser
Prematurely tapping the joystick in order to make the second and third moves is no longer a correct strategy.  These 2 moves now start out by recognizing the first possible input as incorrect.  If you make no move to cross the bridge, Dirk is now killed by electricity instead of the geyser.

Dragon's Lair
The original program gives a buzz sound for many of the incorrect moves that can made in the lair.  Most wrong moves now result in death.  A move U is required after the fourth move.  The disc search error previously caused by moving D at the flashing pillar is now corrected.  The move to grab the magic sword is changed from R or S, to R only.  The move to avoid the dragon's tail is changed from L or U, to L only.  After L to avoid the tail, the next move is now R, because if you watch the animation closely, Dirk specifically moves R in order to squeeze under the dragon's final breath of fire and position himself for the kill.  When the game is completed, the final still frame of Dirk & Daphne is no longer jittery as it always was on a LD-V1000 player.  The death scene of Dirk failing to grab the magic sword now extends into the next scene of Dirk in the flames.

The maximum attainable score with 5 lives is 448,888.

Q & A - WARNING: SURPRISES REVEALED
Q.  Could you alter the drawbridge scene so that if you die in the yellow room, you will restart again in the yellow room?  ...or maybe if you die on the drawbridge a couple times, you are then put into the yellow room?
A.  Splitting the scene into "outside" and "inside" segments doesn't seem possible without incurring some undesirable side effect with the gameplay or its presentation.

Q.  Above, you claim (with exception) that all the animation on the disc is now used, but if you can't lose your last life on the drawbridge, then how do you expect the drawbridge's game-over/skeleton scene to ever be used?
A.  If your game is set to restart after the lair is completed, and you have only 1 or 2 lives left when you restart, you can lose your last life on the drawbridge and see the game-over scene.

Q.  After the Robot Knight, why is a joystick move accepted but not required for the gap in the stairs?
A.  Yes, it initially seems like a falling death scene might go with this segment, but not after you've stopped to think about it.  Unlike the similar-looking collapsing staircase with the bats, there is no threat to Dirk here.  Everything is quiet, nothing is chasing behind him, and the gap is in plain sight right from the start.  There is no reason to believe that Dirk would be stupid enough to walk into the hole on his own.  And, because the gap is always visible, there would be no logic in that moving toward the hole saves Dirk, while making no move causes him to fall in.  Also, no death scene exists for this segment, so it's apparently a simple ending animation with no required move.  Dirk performs many small actions for himself during the game, and this is one of them.

Q.  Why did you just totally remove the original fourth group of scenes... (the two 3-level-falling-platforms & yellow-room-with-3-doors-and-falling-rocks)?
A.  Because the yellow room is now part of the drawbridge as it should be, and because most people do not want to play the falling platform scene 4 times during the same game.  Also because evidence shows that these 3 scenes were not originally intended to exist.  In the ROMs, the indexing data for these scenes is just tacked on at the very end of the master index list for all scenes, (which is otherwise in order).  It's apparent that the 3-level platform & the yellow room were simply added on at the end after it was decided to remove the drawbridge scene from the game.

Q.  Why are the moves changed for the final battle with the lizard king?
A.  The new moves match Dirk's movements and force the final battle to be more interactive.  The original program required only one S after Dirk retrieved his sword, and then you could just watch the rest of the scene play by itself.  Furthermore, the two D moves are nothing new; the game always accepted them.

Q.  Why are the moves changed for the mud men?
A.  Because the actions Dirk performs during the animation demand it.
Second move is now L:  Watch the animation closely.  A line of fire appears on the right side of the screen, and as soon as the video cuts to the next overhead view, Dirk jumps from where he was standing in front of the crater, directly to the left.  Also, the corresponding death scene shows that moving U leads directly to death in the crater.
Fourth move is now R or diagonal U&R:  Dirk moves to the right, and the original program also accepted R and U&R at this point.  U now causes death because U leads over the geyser, and there aren't many other opportunities to use the geyser death scene.
Seventh move is now L or diagonal U&L:  The original program accepts either U or U&L, but the first time I ever got to this point, I went L and died, and I'm still bitter over that.  The flash is clearly to the left.

Q.  You referred to diagonal moves above.  Can you explain?
A.  The game software actually recognizes diagonals as distinct and separate inputs.  Diagonal moves have always existed in some areas of the game where one of the standard directions involved in the diagonal will individually kill you, IE: you could have always moved diagonally U&L (or U&R) to avoid the whirlpools, while U alone would kill you.  It is even possible to define a diagonal U&R move to be correct, and U and R to each be individually incorrect.

EDITOR'S INFO
As of February, 2000, my email is dave@d-l-p.com
Failing this, inquire at www.dragons-lair-project.com
What the heck...  If you like this program ;) please send $10 or so to
Dave Hallock
3911 Winterburn Ave.
Pittsburgh, PA 15207 (USA)
That would be awesome!

ACKNOWLEDGEMENTS
This ROM enhancement is made possible by the help from Robert DiNapoli in deciphering the ROM data.  Also by valuable input from Jeff Kinder and Jeff Kulczycki.  Special thanks to Jeff Kulczycki for the version display.

DISCLAIMERS
I did not write any code contained in these ROMs that is not specifically identified in the above text as my own modification.  The user is solely responsible for any and all adverse effects resulting from the use or misuse of this ROM data or the EPROMs it is stored on.  The ONLY intended application of these ROMs is to be installed into a Dragon's Lair arcade game and used privately by the game's owner.  You are instructed not to use them in any other capacity.