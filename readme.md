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

### Longest and Shortest Wands

### The Rarest Wands

### Cores and Woods by House

### Cores by Blood Status

### Wand Twins

### The Elder Wand Chain

### Does Your Wand Predict Your Fate?

## Discussion

### So, Does the Wand Choose the Wizard?

### Limitations
