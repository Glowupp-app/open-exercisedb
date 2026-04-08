# Open ExerciseDB

**Free open-source fitness exercise database** with **1000+ exercises** in clean, consistent JSON format.

Includes difficulty, primary & secondary muscles, equipment (bodyweight + machines + cables + more), muscle intensity ratings, execution tips, and more.

Perfect for:
- Workout generators & fitness apps
- AI training tools
- Personal trainers
- Research & data projects

### Live Search Demo
Try searching exercises instantly: [Open ExerciseDB Demo](https://demo.glowupp.org)

## Features

- Clean, well-structured JSON schema
- Supports **bodyweight**, **dumbbells**, **barbells**, **machines**, **cables**, **resistance bands**, etc.
- Primary muscle automatically derived from intensity ratings
- Muscle intensity system (P = Primary, S = Secondary, T = Tertiary)
- Fully in English
- Easy to filter and search
- Actively maintained and open for contributions

## Quick Start

```python
import json

with open('exercises.json', 'r', encoding='utf-8') as f:
    exercises = json.load(f)

print(len(exercises))                    # Total exercises
print(exercises[0]['name'])              # First exercise name
print(exercises[0]['primary_muscle'])    # Primary muscle
```
JavaScript example:
JavaScriptfetch('https://raw.githubusercontent.com/Glowupp-app/open-exercisedb/main/exercises.json')
  .then(r => r.json())
  .then(data => console.log(data));
Data Files

exercises.json → Main clean dataset (recommended)
schema.json → Full JSON schema for validation

How to Use
Filter examples:
```
Python# All machine exercises for legs
machine_leg_ex = [ex for ex in exercises 
                  if any("machine" in eq for eq in ex["equipment"]) 
                  and ex["primary_muscle"] in ["Quadriceps", "Glutes", "Hamstrings"]]

# Core exercises with difficulty 7+
hard_core = [ex for ex in exercises 
             if ex["primary_muscle"] == "Abs / Core" and ex["difficulty"] >= 7]
```
Contributing
New exercises (especially machines and cable variations) are very welcome!

Fork the repository
Add or edit exercises following the schema
Run the cleaning script if needed
Submit a Pull Request

See CONTRIBUTING.md for details.
License
This project is licensed under the MIT License — you are free to use, modify, and distribute the data in any project (commercial or open-source). Attribution is appreciated but not required.
Acknowledgments
Originally inspired by Glowupp fitness content. Thank you to all contributors!

⭐ If this helps you, please star the repository!
Keywords: fitness exercise database, workout json, open source gym db, machine exercises dataset, bodyweight exercise list
