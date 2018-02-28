# PFSMM - PathfinderSimpleMonsterMaker

PFSMM creates statblocks for the Pathfinder RPG using Paizo's Simple 
Monster Creation rules. 

* [Simple Monster Creation Rules](http://paizo.com/pathfinderRPG/prd/unchained/monsters/index.html#)
* [Paizo's OGL and Copyright Notice](http://paizo.com/pathfinderRPG/prd/openGameLicense.html)

## Getting Started

Pull down the project and run it from the commandline using python.
Use the -h commandline flag to get the help text.
```
[$] python pfsimplemonstermaker -h
usage: pfsimplemonstermaker [-h] [-c] [-e] [-s] CR

Generate the stats of a Pathfinder monster using the Simple Monster Creation
rules and a given CR.

positional arguments:
  CR                 Set the CR of the generated statblock

optional arguments:
  -h, --help         show this help message and exit
  -c, --combatant    generate a combatant type statblock
  -e, --expert       generate a expert type statblock
  -s, --spellcaster  generate a spellcaster type statblock
```

Currently supports creating a combatant, an expert or spellcaster type 
creature of any (integer) CR of 1 and above. For monsters of a CR rating 
below 1, use "0" as their CR rating.

```
[$] python pfsimplemonstermaker -c 0
Combatant CR 0
AC: 13  Touch: 12  FF: 12 | 10hp  CMD: 15
Fort: 2  Ref: 2  Will: 0 | ADC: 10  SDC: 9
1 +5 skill, 2 +3 skills
1 combat option(s)
Weapon Attacks:
High Weapon: +5 for (5) damage | Low Weapon: +2 for (3) damage
Natural Attacks:
2 at +4 for (6) damage | 1 at +4 for (8) damage, 2 at +-1 for (4) damage

```

## Authors
* **Theodore Mason** - [Domicilius](https://github.com/Domicilius)

## License

This product is licensed under the Attribution-NonCommercial-ShareAlike 4.0 International License - see the 
[LICENSE.md](LICENSE.md) for details.

## Acknowledgements

* [PurpleBooth's README template](https://gist.githubusercontent.com/PurpleBooth/109311bb0361f32d87a2/raw/824da51d0763e6855c338cc8107b2ff890e7dd43/README-Template.md)
* [Paizo](http://paizo.com/) for making Pathfinder RPG and the 
  Simple Monster Creation Rules
