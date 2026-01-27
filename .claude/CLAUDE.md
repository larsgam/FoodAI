# FoodAI - Recipe Collection

## Project Overview

A personal collection of food recipes stored as markdown files in Danish.

## Recipe Format

All recipes must follow this consistent format:

### Structure

```markdown
# [Opskriftens navn]

[Kort beskrivelse af retten - valgfrit]

## Ingredienser (4 personer)

- [mængde] [enhed] [ingrediens], [tilberedning hvis nødvendigt]
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
- Include preparation notes directly on the ingredient line (hakket, skåret i tern, revet, snittet, etc.)
- Example: `- 200 g løg, finthakket`

**Fremgangsmåde:**
- Always numbered steps
- Each step should be a clear, single action when possible
- Use imperative form (steg, rør, tilsæt, etc.)

### Example Recipe

```markdown
# Pasta Carbonara

En klassisk italiensk pastaret.

## Ingredienser (4 personer)

- 400 g spaghetti
- 200 g guanciale, skåret i små tern
- 4 stk æggeblommer
- 100 g pecorino, fintrevet
- Sort peber, friskkværnet

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
