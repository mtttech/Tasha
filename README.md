# Tasha

**Tasha** is a tool for creating 5e Dungeons & Dragons characters.

### Supported rulebooks

  * [*Player's Handbook*](https://www.amazon.com/Players-Handbook-Dungeons-Dragons-Wizards/dp/0786965606/ref=sr_1_1?crid=379ZD2GOSSXUS&keywords=player%27s+handbook+53&qid=1686513995&sprefix=players+handbook+53%2Caps%2C117&sr=8-1)
  * [*Dungeon Masters Guide*](https://www.amazon.com/Dungeons-Dragons-Dungeon-Rulebook-Roleplaying/dp/0786965622/ref=sr_1_1?crid=2OL0NVA15CCB4&keywords=dungeon%2Bmasters%2Bguide&qid=1704477505&sprefix=Dungeon%2BM%2Caps%2C110&sr=8-1&th=1)
  * [*Mordenkainen's Tome of Foes*](https://www.amazon.com/MORDENKAINENS-FOES-Accessory-Wizards-Team/dp/0786966246/ref=sr_1_1?crid=1YK3ZSKRTEC2N&keywords=mordenkainen%27s+tome+of+foes&qid=1686514034&sprefix=mordenkain%2Caps%2C135&sr=8-1)
  * [*Volo's Guide to Monsters*](https://www.amazon.com/Volos-Guide-Monsters-Wizards-Team/dp/0786966017/ref=sr_1_1?crid=9Q6IDI7KI2FH&keywords=volos+guide+to+monsters+5e&qid=1686514111&sprefix=volos%2Caps%2C122&sr=8-1)
  * [*Xanathar's Guide to Everything*](https://www.amazon.com/Xanathars-Guide-Everything-Wizards-Team/dp/0786966114/ref=sr_1_1?crid=1HQBURCPQA50W&keywords=xanathars+guide+to+everything+5e&qid=1686514138&sprefix=xa%2Caps%2C147&sr=8-1)
  * [*Tasha's Cauldron of Everything*](https://www.amazon.com/Cauldron-Everything-Expansion-Dungeons-Dragons/dp/0786967021/ref=sr_1_1?crid=3K7SU399VYTP4&keywords=tasha%27s+cauldron+of+everything+5e&qid=1686514198&sprefix=tas%2Caps%2C118&sr=8-1) - Mostly
  * [*Sword Coast Adventurer's Guide*](https://www.amazon.com/Sword-Coast-Adventurers-Guide-Accessory/dp/0786965800/ref=sr_1_1?crid=JNAGKS1F2Y2U&keywords=sword+coast+adventurer%27s+guide+5e&qid=1686514240&sprefix=sword%2Caps%2C133&sr=8-1) - Partially
  * [*The Wild Beyond the Witchlight*](https://www.amazon.com/Wild-Beyond-Witchlight-Adventure-Dungeons/dp/0786967277/ref=sr_1_1?crid=2UYG545HO9XS7&keywords=The%2BWild%2BBeyond%2Bthe%2BWitchlight&qid=1704650190&sprefix=the%2Bwild%2Bbeyond%2Bthe%2Bwitchlight%2Caps%2C102&sr=8-1&th=1) - Partially

## QUICKSTART

### Dependencies

* [dice](https://github.com/borntyping/python-dice)
* [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit)
* [toml](https://github.com/uiri/toml)

### Installation & Usage

```
# Clone the repository.
git clone https://codeberg.org/mtttech/Tasha.git

# Install the project environment.
cd Tasha
poetry install

# Run the project.
poetry run tasha
```

### Storage Directory

Characters generated by *Tasha* are stored in the following folder, which is created when the program is first run (if necessary).

```
$HOME/.config/tasha/characters
```

### Sample Character

Below is an example of a character TOML file generated by *Tasha*.

```
alignment = "Chaotic Neutral"
allotted_asi = 1
allotted_skills = 2
armors = []
background = "Charlatan"
equipment = [ "Fine Clothes", "Disguise Kit", "Con Tools",]
feats = [ "Athlete",]
features = [ "Sorcerous Origins", "Spellcasting", "Font of Magic", "Metamagic", "Ability Score Improvement",]
gender = "Female"
gold = 80
height = 64
hit_points = 22
initiative = 2
languages = [ "Common", "Elvish",]
level = 4
name = "Asper"
proficiency_bonus = 2
race = "Elf, Drow"
resistances = []
savingthrows = [ "Charisma", "Constitution",]
size = "Medium"
skills = [ "Perception", "Deception", "Sleight of Hand", "Arcana", "Persuasion",]
speed = 30
spell_slots = [ 5, 4, 3,]
tools = [ "Disguise kit", "Forgery Kit",]
traits = [ "Darkvision", "Fey Ancestry", "Keen Senses", "Trance", "Drow Magic", "Drow Weapon Training", "Sunlight Sensitivity", "Superior Darkvision", "Dancing Lights", "Faerie Fire",]
version = "0.3.36"
weapons = [ "Dagger", "Dart", "Light Crossbow", "Sling", "Quarterstaff",]
weight = 108

[bonus]
Dexterity = 2
Charisma = 1

[cantrips]
Sorcerer = [ "Blade Ward (lv. 0)", "Dancing Lights (lv. 0)", "Fire Bolt (lv. 0)", "Chill Touch (lv. 0)", "Lightning Lure (lv. 0)",]

[known_spells]

[prepared_spells]
Sorcerer = [ "Charm Person (lv. 1)", "Tasha's Mind Whip (lv. 2)", "Web (lv. 2)", "Detect Magic (lv. 1)", "Magic Missile (lv. 1)",]

[attributes.Strength]
score = 9
modifier = -1

[attributes.Dexterity]
score = 15
modifier = 2

[attributes.Constitution]
score = 12
modifier = 1

[attributes.Intelligence]
score = 12
modifier = 1

[attributes.Wisdom]
score = 11
modifier = 0

[attributes.Charisma]
score = 16
modifier = 3

[classes.Sorcerer]
hit_die = 6
level = 4
subclass = "Storm Sorcery"
```