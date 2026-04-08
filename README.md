# open-exercisedb

A free, open-source collection of **500+ exercises** (and growing) with detailed information: difficulty, primary/secondary muscles, equipment (including machines), video links, execution tips, and more.

Perfect for fitness apps, workout generators, trainers, researchers, or anyone building fitness tools.

## Features

- Clean, consistent JSON schema
- Supports **bodyweight, dumbbells, barbells, machines, cables, resistance bands**, etc.
- Muscle intensity ratings (P/S/T scale)
- Direct video URLs for most exercises
- Easy to filter by muscle, equipment, difficulty, or category
- Actively maintained and open for contributions

## Quick Start

```bash
# Clone the repo
git clone https://github.com/yourusername/fitness-exercises-database.git
cd fitness-exercises-database

# Load the data (example in Python)
import json
with open("data/exercises.json", "r", encoding="utf-8") as f:
    exercises = json.load(f)

print(len(exercises))        # total exercises
print(exercises[0]["name"])  # first exercise name
