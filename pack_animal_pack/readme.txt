
Pack Animal Pack

A collection of pack animals with a little somethin' somethin'.

-------------------------------------------------------------------------------------------------------------

This pack adds a few new animals with variations, an outfitter, new animal products, and new interactions
between pack animals and some trek members. Still a work in progress with a few more ideas to implement
and some art to complete, but everything currently included is fully functional. Feedback is welcome.

New animals:
Bactrian camels (2 variations)
Goats (3 female + 3 male variations)
Horses (3 variations)

Modified animals:
Camels have been re-classified as Dromedary Camels with modified female variations.
Water Buffalo have modified female variations.

New items include varieties of milk and a couple cheeses.

Milking a dairy animal is done automatigally during travel or waiting, if you have the matching trek member.
You can turn this off by clicking the "Do Not Milk" button on the animal card, when available, and will see the
dairy icon change appropriately. There are some other additions that I'll keep secret, so as not to spoil an
opportunity to discover them on your own. :)


- Goat notes: ~$100, produces about 1 gallon of milk per day, 300 lbs., 75 lbs. carrying capacity
- Donkey notes: ~$600, 200 lbs. carry
- Mule notes: ~$1500, 200 lbs. carry
- Horse notes: ~$2000, pack horse in 1850 was $25, riding horse $75, 300 lbs. live weight carry
- Water buffalo notes: ~$2000, produces milk, about 5 gallons per day, 2000+ lbs,  longer legs, angular bodies,
    shorter horns that curl back and upward into spirals, slow mount, adaptable to most climates.
- Yak notes: ~$2000, Milk producer (similar to goat, 1 gallon per day) and can be combed to collect their wool. 1500+ lbs.,
    650 lbs. carrying capacity, adapted to high altitude and cold weather, will suffer heat exhaustion in warm weather.
- Dromedary camel notes: ~$400, Produces milk, about 5 gallons per day. Cheese is difficult to make from the milk.
- Bactrian camel notes: Produces milk, 1 gallon per day, difficult to make cheese.
- Husky notes: ~$500

TODOs (comtains spoilers):
- The remaining animals: yak, ox, mule.
- Look into using milk for desert movement.
- Now that chat messages are fixed and randomize between characters, add more chat variety based on
    detected personality traits. Cheese to do. Maybe add messages to the goat sacrfice - specifically religious,
    "What have you done?!" "This is an affront to my sensibilities!"
- Look into adding a location check for altars and only add one if needed.
- Consider adding a curse for failure on the cthulhu quest.
- Mutations from the goat quest will need further play testing as they may be underpowered considering their
    rarity, the potential difficulty of the quest, and due to gaining an ailment with them.
- Add particle effects to location tiles to simulate animals grazing.
- Consider adding the barter flavor text when exiting the barter screen. "I noticed the outfitter's
    equipment selection looked rather bare."
- World standing should affect the outfitter's wares on offer. Maybe the price too?
- Consider addding recipes. Khoa is a cheese that can be made easily from buffalo milk in a heated pan, but this cheese
    is usually used in sweets. Maybe if the party has cocoa leaves and milk, make gulab jamun, which is common in
    many regions. Another is barfi, which needs fruit (mangos) or coconut.
- Yak should produce hair bundles, which have small value in trade. Add a harvest wool button, available every 15 days.
- Yak hair can be processed into yarn by a herdsman (animal handler), but let's make mountain troopers more useful
    by having survival skills. Allow them to be able to make the hair into yarn, to produce rope, a blanket
    (which does?), climbing gear (where does the metal come from?), and eventually a tent. Implement with buttons
    for mountain trooper that are available when a yak is in the party, but greyed-out until yarn count conditions
    are met.
- Yaks should suffer heat exhaustion in desert or jungle biomes and eventually die.
- Add "Slaughter for meat" buttons to any pack animal when a bedoiun or native warrior are in the party.
- Fix arctic outfitter event image, there are a couple white pixels on an igloo that force animals to appear
    on it. Happens in the village event image as well.
- Finish the arctic paddock fences by adding gates and snow.
- Add worn, green dirt and sand piles to the nomad event image.
- Add a lizard outfitter location tile and event image.
- Having a lizard shaman will enable egg laying with the parasaurolophus, which can be traded, hatched or made
    into an omelet by a cook.

Ideas that can't be built currently:
- Think about more combo variety for the new mutation dice since these are character attacks:
    tentacle + awareness = parry / disable? - shield and stun weapon dice?
    vclaw_1 + magic = antidote? - small heal, removes poison
- If it can be done, modify the avatar image with the recieved mutations. Specifically add horns and a tentacle.
    And the tentacle could wiggle.

Changelog
v0.3.1.0 - 2019-03-15
-------------------------------------------------------------------------------------------------------------
- Re-factored the milk button to make it more dynamic. It will appear on an animal card only when you have the
  appropriate party member and text will change on each click between "Do Not Milk" and "Milk While Travelling".

v0.3.0.0 - Milk Fountain - 2019-03-07
-------------------------------------------------------------------------------------------------------------
- Added a "(Do / Do not) Milk" button for dairy animals, which will set a dummy status, essentially turning
  off milk production while the party travels. This button will only be available if an animal handler or
  bedouin are in the party.
- Added more milk expiration hacks so traveling with a dairy goat, while not partaking in it's output, doesn't
  result in a flood of milk in the party inventory.
- Changed the outfitter into a true location that can be spawned next to a village. Sublocations didn't allow
  for select or partyEvents, so controlling when they spawn was limited.
- Added outfitter fixture tiles for all biomes.
- Added the remaining base game pack animals to the outfitter, with selections made according to the biome.
- Added a barter animal action, where the player recieves a credit to take from the outfitter inventory.
  This will allow a player to "trade up" one pack animal for another or gather much needed food supplies
  or equipment. Also added an interaction if a player tries to abuse this action by recruiting an animal from
  the village for free, then trying to immediately trade it for goods.
- Bartering a pack animal adds it to the outfitter's purchase stock, limited to 5 animals.
- Purchasing an animal from the outfitter opens a custom event screen where the animals are on display within
  the pen.
- Refactored the camel pack animal as single-humped male dromedary camels.
- Added female dromedary camels and milk.
- Added bactrian camels and milk.
- Refactored the water buffalo pack animal as male water buffalo.
- Added female water buffalo, milk and cheese.
- Added "lite" versions of most pack animals for use in event images. They're assigned the custom2 imgslot
  property, so I have more control over where they spawn, but otherwise have limited properties and no
  crates, so they spawn in bare.
- Added "lite" versions of the camels that are sitting with a saddle, so they don't flip horizontally.
- Added optional chat messages for alcoholics and some personalities drinking milk.

v0.2.0.0 - Urban Goatfitters - 2018-09-21
-------------------------------------------------------------------------------------------------------------
- Added a working outfitter event / location that is spawned with native villages as a sublocation. When an
  outfitter is available, the village will have an Outfitter action that "moves" the party via teleport to
  the outfitter location, which then provides a unique barter inventory as well as a selection of pack
  animals for trade. The goat sacrifice quest would've required a good deal of luck to recruit a goat in a
  village, so this outfitter was added to mitigate that. If the party has the goat sacrifice quest then an
  outfitter will always have at least 1 goat for purchase.
- Tweaks to goat cheese values to make a perfect round more valuable in missions and polar stations. Also
  added autoremove = true since goat cheese would get moldy before the next expedition.
- Added horse and goat chat messages for celebrations.

v0.1.0.0 - Initial build - 2018-09-07
-------------------------------------------------------------------------------------------------------------
- Combined the goat and horse mods into an organized single large mod, using corrupted lands as an example.
