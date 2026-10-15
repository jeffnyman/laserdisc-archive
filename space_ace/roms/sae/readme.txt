SPACE ACE ENHANCEMENT ROM SET VERSION 1.0 · April 9, 2002
Dave Hallock · dave@d-l-p.com

These ROMs contain radical functional changes that require the following text.
This complete document must accompany all distribution of these ROMs.
Mandatory information for proper installation and operation follows.

INTRODUCTION
This ROM set has been created to enhance the gameplay of Cinematronics' 1983 arcade version of Space Ace.  Logical reconstruction to game organization and presentation has been implemented, and the result is what is believed to be the first and only Space Ace game program that plays the game the way it was intended to be played while it was being designed/animated (on cadet skill level).

ROMS
SAE occupies 5 type 2764 EPROMs or compatible.  There is one set of SAE.  It works with any working Cinematronics SA game using any laser disc player.  The creation of different SAE ROM sets optimized for different laser disc players was not necessary.  These ROMs' internet home is www.dragons-lair-project.com/tech/enhancements/sae.asp  Check there to see if any updates exist.

SETTINGS
All of the DIP switch functions & settings for SAE have been remapped to match those of Dragon's Lair.  Generally speaking, whenever SAE ROMs are swapped for DL or DLE ROMs, no DIP switch adjustments are required to keep the same game settings.

New DIP switch features include:
· skill level selection (to benefit users without control panel skill level buttons)
· 1 coin per credit option
· a new game difficulty option

Note: The DIP switches on the main PCB are numbered from 0-7, not 1-8.

SAE DIP switch settings chart:

·······································································
A. Attract Mode Sound
     Always on ··························· B0=ON,  B1=ON  (RECOMMENDED)
     Plays every 8th time ················ B0=OFF, B1=ON
     Always off ·························· B1=OFF

B. Number of Coins Required for One Credit
     2 ··································· A0=ON,  A4=ON  (RECOMMENDED)
     1 ··································· A0=OFF, A4=ON
     2 credits at all times/free play ···· A4=OFF

C. Number of Lives Per Credit
     3 ··································· A5=ON,  B2=ON
     5 ··································· A5=OFF, B2=ON  (RECOMMENDED)
     Unlimited lives for testing purposes  B2=OFF

D. Playtest and Diagnostics
     Normal operation ···················· A3=ON,  A7=ON  (RECOMMENDED)
     Playtest for engineering use ········ A3=OFF
     To run diagnostics, set A7 to ON, and
       power up the game.  After you hear
       two beeps, turn A7 to OFF.  Turn A7
       back to ON to end diagnostics. ···· A7=first ON, then OFF

E. Game Difficulty Level*
     Normal: when a life is lost, gameplay
       resumes immediately after the point
       the player died.  The fatal move is
       not replayed. ····················· B7=OFF (RECOMMENDED)
     Hard: when a life is lost, gameplay
       resumes back at the beginning of
       the scene.  All moves must be
       replayed. ························· B7=ON  (DISCOURAGED)

F. Skill Level Selection
     Normal Mode (control panel skill
       level buttons are enabled) ········ B5=ON,  B6=ON  (RECOMMENDED)
     Always SPACE ACE skill level ········ B5=ON,  B6=OFF
     Always CAPTAIN skill level ·········· B5=OFF, B6=ON
     Always CADET skill level ············ B5=OFF, B6=OFF

G. Disc Player Model Selection
     Pioneer PR-7820 ····················· B3=ON
     Pioneer LD-V1000 ···················· B3=OFF (MOST COMMON)
·······································································

Not Used: A1, A2, A6, B4

Note: The original Space Ace DIP switch option for "enable frame display" is no longer available.

*Warning: The hard difficulty option is not recommended and should not be used.  It requires players to learn & master each & every move of the game in sequence before progressing to any new gameplay.  New players will quickly abandon such a game.  Our beta tests proved that SAE must be set to normal difficulty in order to hold the interest of new players.  A preferred means of difficulty increase is to use the 3 lives option, whereas players can only make 2 mistakes.  (The game difficulty DIP switch setting applies to all 3 skill levels.)

SCORE CHART
SAE has a new and structured scoring scheme:

·······································································
Making a correct move ·············· as Dexter · as Space Ace
· during the 1st third of the game       586          782
· during the 2nd third of the game       906        1,208
· during the 3rd third of the game     1,402        1,868

Energizing · 1,500

Shooting enemies*:
robots and mechanical weaponry · 2,000 each
asteroids · 1,500 each
space station video guards · 4,000 each
animal or marine creatures:
· small  · 500 each
· medium · 2,500 each
· large  · 3,500 each
alien spaceships · 10,000 each
Le Grins · 2,500 each
Hexter · 5,000
*score is awarded for direct hit to enemy, whether destroyed or not

Defeating Borf · 25,000

? · 35,000
·······································································

ENHANCEMENTS
Video
All animation recorded on the laser disc is now used by the game program.

Smoother video transitions exist everywhere that a disc player search is executed.

Diagnostics
The diagnostics messages now remain on-screen long enough to be read.

Attract Mode
The DIP switch option to play the attract mode audio only 1 out of 8 times now plays the audio on the first time after power-up, instead of the 8th time after power-up.

When a coin is dropped, the screen freezes on the pricing & lives per game information, instead of the Space Ace title screen.  If a start button is then pressed while the game contains only partial credit, a text message instructing to "deposit another coin", or "more coins" (as appropriate) is briefly displayed.

Game Mechanics
When a 1-player game ends due to all lives lost, the "player one game over" message will be displayed after Borf's final appearance.  Originally, the attract mode resumed immediately.

During a 2-player game, if one player completes the game, the message which warns of player change will be displayed.  Originally, the remaining player's game continued abruptly without warning.

Gameplay
- Presentation
All quirks, bugs, and discontinuities characteristic of Space Ace have been eliminated.  This was accomplished by deleting ALL of the original game data.  SAE gameplay has been written entirely from scratch.  Absolutely no part of the original Space Ace game data exists in SAE.

When the game accepts an incorrect move, you will hear the "move accepted" beep.  The original Space Ace plays a buzz when it accepts a wrong move, resulting in ambiguity as to whether the move was incorrect or just poorly timed.  Dragon's Lair plays the beep whenever any move is accepted, whether correct or not.  This behavior is more beneficial and has been duplicated in SAE.  When the beep plays for an incorrect move, you'll know for sure that your move was accepted, and that it was wrong, and not to try it again.

With all 3 skill levels, scenes are presented once per game, with the orientation randomly selected.  A game of SAE will never require you to play both a scene and the reverse of that same scene during the same game, either in whole or in part.

All score values for shooting enemies are added into the score display at the exact moment that the target explodes!

At every opportunity to energize during the game, (except during the final scene), a flash indicates an alternate route that may be taken instead of energizing.  If you choose not to energize and play as Dexter, you must move the joystick in this alternate direction.  You cannot simply do nothing, as the original program often allows.  If you neither energize nor move anywhere, you will lose a life (except during the final scene).

If you do not initially energize during the final scene, Dexter receives repeated cues to energize while continuing to play out the motions of the fight with Borf that Ace would have gone through.  When you finally choose to energize, Ace's fight with Borf will pick up at the point that Dexter's fight left off.

- Skill Levels
The SAE skill levels add a new dimension!  Each skill level presents a uniquely distinct way to play Space Ace.  Hopefully you will find each SAE skill level equally entertaining, and maybe even have trouble deciding between them every time you start a game.

· CADET · This is the normal game, conforming to what is believed to be the original game design theory.  A complete game contains 10 of the 13 scenes on the laser disc.  The exits that you choose at the end of certain scenes determine which scenes are played next, and which scenes are left out of the game.  More details on this are below.

· CAPTAIN · This game is like CADET, except that all 13 scenes on the disc are played in a complete game.  As in the CADET game, CAPTAIN allows the same occasional opportunities to choose what the next scene will be, based on the exit path you take; however, the scene you do not choose will then follow immediately after the one chosen, instead of being left out of the game.

· SPACE ACE · Like CAPTAIN skill, all 13 scenes are played in one complete game.  But additionally, whenever you choose to energize and play Ace's path through a scene, after Ace changes back into Dexter, you will then also immediately play some or all of Dexter's path through that same scene.  If you initially choose not to energize, then you will only play Dexter's path through the scene, and never Ace's.  To play both paths, you must energize.  (Playing both paths does not occur during the last 3 scenes.)

· Summary
· CADET · normal, plays 10 of 13 scenes
· CAPTAIN · plays all 13 scenes
· SPACE ACE · plays all 13 scenes, both Ace's & Dexter's paths

If your system does not include the 3 control panel skill level buttons, you can manually select the skill level as outlined in the DIP switch settings chart above.  Doing so disables all use of the control panel buttons.

- Choosing Your Path Through the Game
This section reveals the methods of scene selection and any associated strategies, shortcuts, or means of game manipulation.  Although it is recommended to read and know the following information, the daring may wish to play SAE first.

When Dexter encounters two exits at the end of a scene, the exit chosen will determine what scene will play next.  Here is how to choose the scene you want to play:

· The First Star Pac Flight: At the end of this scene, you can choose where to land the Star Pac on the space station.  If you choose to land near Borf's ship, the next scene will be the hallways with the power cylinders and video guards.  If you choose to land in the empty landing pad, the next scene will be the red security spheres and the flying platforms.

· On Space Station Level 1*: If you exit through the left portal, the next scene will be the green space pups & giant robot guards.  If you exit through the right portal, the next scene will be the trash masher.  (It doesn't matter if the scene is reversed or not; left and right always remain constant.)
*The power cylinders scene & the flying platforms scene are both on "Space Station Level 1".  The space pups scene & the trash masher scene also both take place on the same space station.

· The Second Star Pac Flight: Dexter leaves the space station via the Star Pac and engages in a dogfight.  On CADET skill level, the following scene will then randomly be either the checkered tunnel with the Le Grins, or Shag's jungle; you are unable to choose.  However!, there is a shortcut in the tunnel during the dogfight that will take you directly to the checkered tunnel scene.  Move horizontally into the tunnel instead of up to fly outside.  (This shortcut ends the high-scoring dogfight scene halfway through.)  For CAPTAIN and SPACE ACE skills, the dogfight scene is always followed by the checkered tunnel, followed by Shag.

Remember, when playing CAPTAIN or SPACE ACE skill levels, the scenes you do not choose will immediately follow the scenes you do choose.  For example, if you land the Star Pac next to Borf's ship and play through the power cylinders, then regardless of which exit portal you choose, the next scene would be the flying platforms.  The exit portals at the end of the flying platforms would then allow you the next scene selection.

- New Moves
This paragraph explains the moves in SAE that differ from the original SA.  You may wish to complete SAE on your own before reading it.  |  This text will explain only the substantially different new moves in SAE.  There are 9 of them.  1. You must move left towards the Star Pac when Ace falls down beside it.  2. You must move left or right to choose where to land the Star Pac on the space station.  3. You must move up during the overhead view of the space pups charging Ace from each side.  4. Near the end of the space pups scene, you must move horizontally when the floor flashes while Ace runs away from the flames shooting at his back.  5. The last move of the space pups scene, for both Dexter and Ace, is now horizontal instead of up.  6. The last move of Dexter's path through Shag's jungle is either left or right to choose a tunnel, while avoiding the bobbing purple carnicula.  7. Ace's last move of the motorcycle chase is to fire.  8. You must fire when Ace's thumb buttons flash underwater.  9. You must move down or press fire when Borf conspicuously leans back on one foot to kick Ace in the head. · There are other minor alterations & directional constrictions to some moves throughout SAE that are simple enough to skip discussing here; just follow the flashes.  There are also a few fun optional new moves that match the action in the animation but do not award score.

Q & A · (NO SECRETS REVEALED)
Q. Why do I see the letter H in parts of the score display?
A. If you do not have a Space Ace annunciator PCB (which lights the skill level LEDs) connected to your game, the letter H regularly appears in the score display.  This is because the signals meant for the annunciator board continue through to the score display if the board is not there to intercept them.  This same effect is generated by the original SA ROMs also.

Q. When I die on a move where I'm supposed to shoot something, my next life begins by showing Dexter/Ace shooting that thing, but I don't get any score for it.  Is that correct?
A. That's correct.

Q. Which parts of the laser disc were never used by the original game?
A. The segment of the Star Pac landing in the empty landing pad of the space station, the segment of Dexter rocking back and forth in front of the ladder at the end of the trash masher scene, and Dexter's last roll to the right to avoid Borf during the final scene, were never accessed by the original Space Ace game.

Q. Do the different skill levels have any effect on the difficulty of the game?
A. No.  The 3 skill levels, CADET, CAPTAIN and SPACE ACE, have no effect on the difficulty of timing moves.  The original program's CAPTAIN and SPACE ACE skills automatically shortened the time windows for making each move.  The results of this were quite sloppy.  SAE's 3 skill levels also have no effect on where your next life resumes after you die.  That function is handled by DIP switch B7 alone.

Q. When I win the game, why do I see the ending video play one frame too many after the black circle closes up on the Space Ace title?
A. If you've disabled the attract mode sound, then unfortunately, that is the moment when the mute command is sent to the disc player.  This takes additional time and causes the ending video to overrun by one frame before the search for the attract mode is executed.  SAE is timed to end the video perfectly when attract mode sound is enabled.

Q. What's a Star Pac?
A. It is the name of Dexter's spaceship.

CREATOR'S INFO
Dave Hallock
As of April 2002, my email is dave@d-l-p.com
Find more of my ROM enhancements at www.dragons-lair-project.com

ACKNOWLEDGEMENTS
Considerable technical assistance, and new game mechanics, DIP switch & coinage features provided by Jeff Kulczycki.  Additional assistance and consultation by Jeff Kinder, Warren Ondras and Matt Ownby.  Special thanks to Rob DiNapoli's initial work in this area.

DISCLAIMERS
The user is solely responsible for any and all adverse effects resulting from the use or misuse of this ROM data or the EPROMs it is stored on.  The ONLY intended application of these ROMs is to be installed into a Space Ace arcade game and used privately by the game's owner.  You are instructed not to use them in any other capacity.