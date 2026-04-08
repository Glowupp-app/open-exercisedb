<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Open ExerciseDB - Free Fitness Exercise Database",
  "description": "Comprehensive open-source JSON dataset with 1000+ fitness exercises. Includes primary & secondary muscles, difficulty level, equipment (bodyweight + machines), muscle intensity ratings, execution tips, and more. Perfect for workout generators, fitness apps, AI tools, and trainers.",
  "url": "https://github.com/Glowupp-app/open-exercisedb",
  "license": "https://opensource.org/licenses/MIT",
  "keywords": [
    "fitness", "exercise", "workout", "exercise database", "fitness database", 
    "json dataset", "strength training", "bodyweight exercises", "gym exercises", 
    "machine exercises", "core workout", "open data", "workout api", "fitness json"
  ],
  "creator": {
    "@type": "Person",
    "name": "Glowupp-app",
    "url": "https://github.com/Glowupp-app"
  },
  "datePublished": "2026-04-08",
  "version": "1.0.0"
}
</script>

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
