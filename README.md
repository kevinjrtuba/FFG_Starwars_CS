# Roll20 FFG Star Wars Character Sheet

## Change log
* 6.1.0
  * Debut of the new suggestions feature. Upon rolling a general skill, or custom skill whose name matches a general skill name, the system will now prompt you for ways to spend the results of your roll.
    * Beneficial results like success, advantage and triumph suggestions will be whispered to both the GM and any players controlling the rolling character.
    * Harmful results like failure (if applicable), threat and despair suggestions will only be whispered to the GM to help cut down on player meta gaming.
  * Added new species and specializations
  * Collapsing sections now respect last state.
  * Fixed bugs in NPC force skills
  * Fixed armor section in stat block for both starships and planetary vehicles
  * Added the skills Survival and Athletics to the Riding Beasts skill list
  * Fixed the version number for the js and css files
  * Fixed some HTML bugs
* 5.7.2
  * Changed to use the Semantic versioning way of doing the versioning labels.
    * For more information on what this means please visit: http://semver.org/
  * Shrunk NPC tab to two tabs: NPC and Critical Injuries
    * Replaced Talents and Abilities with a single textarea
    * Added Equipment as a textarea section
    * Reduced skills to Cool, Vigilance, Combat Skills and five custom skills
    * Changed the initiative dice calculators to just echo what the actual skills have for their dice calculations to reduce the number of times this has to be entered..
    * Added NPC Type to NPC Info
    * Added ability to collapse all npc sections to just one line each
  * Fixed some invalid html attributes
  * Corrected indenting for all the html
  * All companion sections can now shrink to one line.
  * Added back initiative for riding beast and fixed problems it had before.
  * Removed skills from the riding beast's attack drop down that weren't included in the riding beast's skills section.
  * Increased the player's force threshold from 9 to 21.
* 5.0.6.2
  * Moved the Dice and Destiny section below the sheet type selectors but still displayed on all sheets in order to maintain visual flow as much as possible.
  * Added the ability the shrink the whole section down to one line similar to the initiative sections. The individual sections are still collapsible. Will do the same for the other sections because now I agree that sometimes you just want to be able to just completely get rid of a section.
* 5.0.6.1
  * Added support for individual weapons collapsing
* 5.0.6.0
  * In an effort of making the dice and destiny pool more accessible as well as to make progress on the ongoing project of cleaning up and optimizing the code base I have moved them above the sheet type selectors. Now from any sheet you can access those two sections. This also removes sections of duplicated code.
  * Changed the planetary vehicle hard points box to be a number type instead of a text type to fall in line with the space vehicle.
  * Fixed the spacing on the force threshold and committed labels.
* 5.0.5.0
  * The vehicle sheet is now finished with the collapsing project.
  * All sections are now complete in being collapsible.
  * Removed the Riding Beast's initiative section in an effort to optimize and reduce the code base where possible.
    * While yes I can see reasons why someone would want their riding beast to act on a turn other than theirs, the reality is that this is probably a huge minority of players and mechanically the riding beast would work just as well acting on the turn of the owner.
    * From a code base perspective this didn't really feel like a huge necessity to warrant the code hit in keeping around.
  * Removed all weapon skills from the riding beasts attack drop down save for Brawl and one Custom Skill in a effort to reduce and optimize the code base.
    * This was done for the following reasons:
      1. Most riding beasts will only be able to use brawl as an attack skill.
      2. The other weapon skills weren't listed on the riding beast's skill list so the corresponding skills in the attack skill dropdown wouldn't have even worked.
      3. If there is a skill other than Brawl that you want the Riding beast to be able to use for fighting that is what the Custom Skill 1 is for.
  * Removed the old vehicle section in an effort to reduce and optimize the code base.
  * Added a collapsing section to the version info at the top of the sheet so that it can be hidden at will. By default it is hidden.
  * Removed the explanation of recent changes in the version section in an effort to reduce and optimize the code base. Provided a way to get here in order to provide a much more in-depth and current change log.
* 5.0.4.0
  * Finished adding collapsing sections to the Character, companion and NPC sheets.
  * Next update to add collapsing sections to the Vehicle and Group sheets on the player handouts.
  * Changed the color of the repeating section buttons to match the color of the table headers to tie them in better with the color scheme of the sheet.
* 5.0.3.0
  * All section headers on the character's tab are now collapsible where it makes sense. If you see a click cursor on a section header you can collapse it. This should make it much easier to assess what information is available.
  * Removing reliance on break tags where possible allowing for a more natural flow of the document as items are added to repeating sections.
  * Brought the initiative section's look and feel up to the level of the other sections.
  * **Warning** Since the old vehicle section has been officially deprecated for a while I will be removing it in its entirety soon.
    * If you haven't transferred your data by now the attributes that contain them now will still contain them then but you will have to go to the attributes on the attributes page yourself and get the data.
  * Dice pool and destiny section can also be collapsed on the Character, NPC and GM pages.
* 5.0.2.0
  * NPC sections headers are now collapsible when there is more than one section header on a page.
* 5.0.1.0
  * All section headers on the -DiceRoller sheet are now collapsible by clicking on their name.
  * Force powers should be working and pulling from the right sources.
  * Expanded the companion skills to a full skill section.
* 5.0.0.1
  * Fixed npc sheet's collapse sections.
  * Added expense field to group resources.
* 5.0.0.0
  * New NPC sheet for gm's to use in order to make creating npcs easier.
  * Fixed companion initiative.
  * Fixed character and companion weapon attachment.
  * Added more upgrade slots to force powers for character and companion.
  * Fixed spacing for armor header.
  * Changed tab clicked and neutral colors to make them easier to read and understand.
  * Fixed hitbox for long selectors (thanks Vince!).
  * The footer visibility can now be toggled but it will stay to assist people in getting the help they need.
  * Reverted the initial class and specialization to a text box until roll20 supports the DataList HTML5 tag.
* 4.0.4.12
  * Added optgroups to companion career and specialization.
  * Fixed initiative not handling custom items well.
  * Fixed Lightsabers not rolling when used as combat skills (thanks Tim P.).
  * Fixed critical rolls going below 1 and failing to output. Critical rolls will now always result in a minimum of 1.
  * Added page footer.
* 4.0.4.11
  * Closed some html tags that weren't properly closed.
  * Added Medicine to weapons.
  * Added three more attachment slots to weapons as a stop gap before I can get them turned into an actual repeating table.
* 4.0.4.10
  * Added the ranged (light) and ranged (heavy) skills to the available skills for the force powers.
  * Added resilience to the weapons dropdown skills to account for the ithorian race being able to bellow.
  * Changed the first career and specialization to be a dropdown.
  * Characters, Companions, Beasts, Starships, and Planetary Vehicles all have working separate critical tables now.
