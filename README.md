# open-exercisedb

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Open ExerciseDB - Free Fitness Exercise Database",
  "description": "Comprehensive open-source JSON dataset with 1000+ fitness exercises. Includes primary & secondary muscles, difficulty level, equipment (bodyweight + machines), muscle intensity ratings, execution tips, and more. Perfect for workout generators, fitness apps, AI tools, and trainers.",
  "url": "https://github.com/YOURUSERNAME/open-exercisedb",
  "license": "https://opensource.org/licenses/MIT",
  "keywords": [
    "fitness", "exercise", "workout", "exercise database", "fitness database", 
    "json dataset", "strength training", "bodyweight exercises", "gym exercises", 
    "machine exercises", "core workout", "open data", "workout api"
  ],
  "creator": {
    "@type": "Person",
    "name": "Zan",
    "url": "https://github.com/Glowupp-app"
  },
  "datePublished": "2026-04-08",
  "version": "1.0.0"
}
</script>
A free, open-source collection of **300+ exercises** (and growing) with detailed information: difficulty, primary/secondary muscles, equipment (including machines), execution tips, and more.

Perfect for fitness apps, workout generators, trainers, researchers, or anyone building fitness tools.

## Features

- Clean, consistent JSON schema
- Supports **bodyweight, dumbbells, barbells, machines, cables, resistance bands**, etc.
- Muscle intensity ratings (P/S/T scale)
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
```
Data Structure
See schema.json for the full specification.
Main file: data/exercises.json (array of exercise objects)
Example filter (Python):
# All machine exercises for quads
machine_quads = [ex for ex in exercises 
                 if "machine" in ex["equipment"] 
                 and ex["primary_muscle"] == "Quadriceps"]

How to Contribute

Fork the repository
Add new exercises following the schema (or improve existing ones)
Run the validation script: python scripts/validate.py
Submit a Pull Request

New exercises welcome — especially machine-based ones, cable exercises, and variations!
See CONTRIBUTING.md for details.
License
This project is licensed under the MIT License — you are free to use, modify, and distribute the data in any project (commercial or personal). Attribution is appreciated but not required.
Acknowledgments
Originally inspired by Glowupp fitness content. Thank you to all contributors!

⭐ Star this repo if you find it useful!
