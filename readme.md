# Does the Wand *Really* Choose the Wizard?

## Introduction

*"The wand chooses the wizard."* — Mr. Ollivander

In Harry Potter, wands are more than tools. They tie characters together. Harry's and Voldemort's wands are "brothers," made with feathers from the same phoenix. Neville struggles with his father's wand until he finally gets one that chooses him. And the Elder Wand, first owned by Antioch Peverell, passes from wizard to wizard through defeat, driving Grindelwald and Voldemort to obsession.

At Hogwarts, the closest thing to data analytics is Arithmancy and Ancient Runes. As a Muggle, I traded dusty tomes for code. Using character data from PotterDB, I set out to see whether the wand really chooses the wizard.

From the first wand at Ollivanders to the final duel, I explored:

- The Elder Wand chain
- Cores by house
- Woods by house
- Blood status and cores
- Rarest wands
- Wand twins
- Longest and shortest wands
- Wands and survival
  
## Data

I pulled character data from the PotterDB API in Python and kept only characters who appear in the books and have a known wand. That left X characters out of Y total.

For each character, I used:

- **Wand:** wood, core, and length
- **House:** Gryffindor, Hufflepuff, Ravenclaw, or Slytherin
- **Blood status:** pure-blood, half-blood, or Muggle-born
- **Birth date**
- **Died / survived**

Some characters had more than one wand, so I kept each character's main wand, the one they used most in the books. For Neville, that's his own wand, not his father's.

### Turning Wand Lore into Data

PotterDB stores each wand as one line of text, like `11", Holly, phoenix feather`. To analyze it, I:

- Split the text into separate wood, core, and length columns
- Standardized core names so variations like "phoenix feather" and "phoenix tail feather" match
- Converted length to a number in inches, leaving it blank when it wasn't listed

## Methods

## Results


### Cores by House

Gryffindor (brave, daring, chivalrous): An even split between unicorn hair and dragon heartstring, plus phoenix feather and the only thestral hair wand. This suggests a house whose bravery balances doing the right thing with the power to act boldly, since unicorn hair is the hardest core to turn dark and dragon heartstring is the most powerful.

Hufflepuff (loyal, patient, hardworking): One unicorn hair and one phoenix feather wand, with no dragon heartstring. This suggests a house whose magic comes from steadiness and earned trust rather than raw power, since both cores reward an owner who's consistent and patient.

Ravenclaw (wise, witty, curious): An even split between dragon heartstring and unicorn hair. This suggests a house that loves learning quickly but still values thinking things through, since dragon heartstring learns the fastest and unicorn hair keeps the magic steady.

Slytherin (ambitious, cunning, resourceful): The only house led by dragon heartstring, with a mix of four different cores, including the only basilisk horn wand, a fitting core for the house of the serpent. This suggests a house that sees power as a tool, choosing the strongest core and accepting its temper to get ahead, while staying resourceful enough to use whatever works.

The houses share more than the rivalries suggest, so the same few cores show up in all of them. With only 2 to 9 canon wands per house, these are patterns worth noting rather than firm conclusions.

<img width="1600" height="1000" alt="image" src="https://github.com/user-attachments/assets/60b742e4-f42f-4fe0-abc1-7abfb5cd727e" />

### Woods by House

Willow, ash, and holly were the most common woods, but no wood appeared in more than 5 wands, and most showed up only once or twice. There were 21 different woods compared with just 5 cores, and while cores showed some loose patterns by house, wood showed none at all. That makes sense, since a wand's wood connects to a person's own magic, and no two witches or wizards have the same magic. Your house is something you share, but your wood is yours alone.

<img width="1600" height="1000" alt="image" src="https://github.com/user-attachments/assets/acf4552b-af00-4dcf-9450-4a3d1bee193a" />

### Cores by Blood Status

Blood status is one of the biggest dividing lines in Harry Potter, with pure-blood supremacy driving the whole Death Eater ideology. But when I compared wand cores across blood status, the three groups looked surprisingly similar. Unicorn hair made up the largest share in every group, and dragon heartstring, the most powerful core, showed up in all three, including Muggle-borns. The small differences, like pure-bloods having slightly more phoenix feather, come down to a few individual characters rather than a real pattern. The Muggle-born group only has 2 wands, so it can't show much on its own, but it does show that Muggle-borns aren't shut out of powerful cores. Blood status divides the wizarding world, but not its wands.

<img width="1600" height="1000" alt="image" src="https://github.com/user-attachments/assets/1b181d0a-d1b9-40cf-8263-549d5d5dfb8d" />

### Longest and Shortest Wands


### The Rarest Wands


### Wand Twins



### The Elder Wand Chain

The Elder Wand changed hands 13 times, from Antioch Peverell to Harry Potter, across every era from Ancient to Modern. Most of its masters won it by defeating, or even killing, the owner before them, since the wand's loyalty goes to whoever beats its current master. The chain ends with Harry, the only master who won it without trying to and chose not to keep using it.

<img width="2400" height="800" alt="image" src="https://github.com/user-attachments/assets/dfb777f2-ae78-4d9d-9252-6f7ccf95d79b" />


### Does Your Wand Predict Your Fate?





## Discussion

### So, Does the Wand Choose the Wizard?

### Limitations
