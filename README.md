# Lair Dramatic Presentation Scorer

A scalar function that evaluates the theatrical and aesthetic potential of locations as villain lairs, returning a score from 0 (mundane, unsuitable) to 1 (magnificently theatrical).

## Overview

Great villain lairs are more than practical hideouts—they're stages for theatrical villainy. This function evaluates locations across four dimensions that contribute equally to the final score:

1. **Architectural Grandeur (25%)** - Scale, natural feature integration, ceremonial spaces, and visual dominance
2. **Atmospheric Quality (25%)** - Natural mood enhancement, lighting potential, acoustics, and atmospheric effects
3. **Symbolic Resonance (25%)** - Historical associations, mythological significance, ironic potential, and iconic memorability
4. **Monologue Backdrop Quality (25%)** - Dramatic gesture views, human figure framing, environmental punctuation, and backlighting potential

## Input

```json
{
  "location": "A text description of the location",
  "villain_profile": "Optional: villain's aesthetic preferences for calibrated evaluation"
}
```

### Parameters

- **location** (required): A text description of the location, from brief phrase to detailed architectural description
- **villain_profile** (optional): Description of the villain's aesthetic preferences, power source, era affinity, and desired emotional register. When provided, evaluation is calibrated to this specific villain type.

## Output

A scalar value between 0 and 1:

- **0.85-1.0**: Legendary lair potential - Volcanic fortresses, Gothic castles on stormy cliffs, orbital stations with planetary views
- **0.65-0.85**: Excellent lair potential - Abandoned cathedrals, submarine bases, repurposed missile silos
- **0.45-0.65**: Competent lair potential - Industrial facilities, remote mansions, converted bunkers
- **0.25-0.45**: Marginal lair potential - Generic office buildings, standard warehouses, suburban homes
- **0.0-0.25**: Unsuitable - Daycare centers, community gardens, cozy bed and breakfasts

## Examples

High-scoring locations:
- Obsidian fortress in an active volcano caldera (0.95+)
- Abandoned Gothic cathedral with lightning rods and deep crypts (0.85+)
- Space station in geostationary orbit with Earth views (0.80+)

Low-scoring locations:
- Strip mall in suburban New Jersey (0.15)
- Victorian mansion converted to daycare center (0.20)
- Cozy bed and breakfast with fresh-baked cookies (0.10)

## Evaluation Criteria

The function uses 17 specialized evaluators across the four dimensions:

### Architectural Grandeur
- Scale and Intimidation
- Natural Feature Integration  
- Ceremonial Space Potential
- Visual Dominance and Silhouette

### Atmospheric Quality
- Natural Mood Enhancement
- Lighting Potential
- Acoustic Properties
- Atmospheric Effects Potential

### Symbolic Resonance
- Historical and Power Associations
- Mythological and Archetypal Significance
- Ironic and Subversive Potential
- Iconic Memorability

### Monologue Backdrop Quality
- Dramatic Gesture Views
- Human Figure Scale and Framing
- Environmental Punctuation and Dramatic Beats
- Backlighting and Silhouette Potential

A final holistic assessment integrates all dimensions to ensure dimensional harmony.

## Use Cases

- Evaluating fictional locations for storytelling
- Scoring real architectural sites for dramatic potential
- Comparing multiple candidate locations for theatrical impact
- Understanding what makes spaces cinematically compelling
