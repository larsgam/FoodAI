# FoodAI - Recipe Collection

## Project Overview

A personal collection of food recipes stored as markdown files in Danish.

## Recipe Format

All recipes must follow this consistent format:

### Structure

```markdown
# [Opskriftens navn]

[Kort beskrivelse af retten - valgfrit]

Kilde: [URL eller bogref - kun hvis oplyst af brugeren]
Tid: [tilberedningstid - hvis oplyst i kilden]

## Ingredienser (4 personer)

- [mængde] [enhed] `[ingrediens]`, [tilberedning hvis nødvendigt]
- ...

## Fremgangsmåde

1. [Første trin]
2. [Andet trin]
3. ...
```

### Rules

**Ingredienser:**
- Always scaled to 4 persons (recalculate if original recipe is for a different number)
- Written as bullet points
- Use metric units (gram, kg, ml, dl, liter, cm)
- Highlight ingredient names with backticks for visual emphasis
- Include preparation notes directly on the ingredient line (hakket, skåret i tern, revet, snittet, etc.)
- Example: `- 200 g `løg`, finthakket`

**Fremgangsmåde:**
- Always numbered steps
- Each step should be a clear, single action when possible
- Use imperative form (steg, rør, tilsæt, etc.)

**Kilde:**
- Only include if the user provides the source (URL, book name, etc.)
- Place on its own line directly before the ingredients section
- Format: `Kilde: [source]`

**Tid:**
- Include if the source specifies preparation/cooking time
- Place on its own line after the source, before the ingredients section
- Format: `Tid: [time]` (e.g., "Tid: 45 min" or "Tid: 2 timer")

**Brød og dej:**
- For recipes with bread dough, always include hydration percentage in the description
- Hydration = (water weight / flour weight) × 100
- Example: "Hydration: 87%" or include in description like "En dej med 87% hydration"

### Example Recipe

```markdown
# Pasta Carbonara

En klassisk italiensk pastaret.

Kilde: Valdemarsro
Tid: 30 min

## Ingredienser (4 personer)

- 400 g `spaghetti`
- 200 g `guanciale`, skåret i små tern
- 4 stk `æggeblommer`
- 100 g `pecorino`, fintrevet
- `Sort peber`, friskkværnet

## Fremgangsmåde

1. Kog pastaen i rigeligt saltet vand efter anvisningen på pakken.
2. Steg guancialen på en tør pande ved medium varme til den er sprød.
3. Pisk æggeblommer og revet ost sammen i en skål.
4. Vend den drænnede pasta i panden med guancialen (væk fra varmen).
5. Tilsæt æggeblandingen og vend hurtigt rundt.
6. Server straks med ekstra revet ost og friskkværnet peber.
```

## File Organization

- Store recipes as `.md` files
- Use descriptive filenames in lowercase with hyphens: `pasta-carbonara.md`

## Converting Recipes

When transforming recipes from the internet or prompts:
1. Translate to Danish if needed
2. Recalculate all quantities to serve 4 persons
3. Convert all measurements to metric
4. Add preparation notes to ingredients
5. Format steps as numbered list
6. Ensure consistent formatting

## Git Workflow

After creating or updating a recipe file, always execute the following Git commands:
1. `git add [filnavn]` - stage the new/changed file
2. `git commit -m "Tilføj/Opdater opskrift på [navn]"` - commit with descriptive message
3. `git push` - push to GitHub
