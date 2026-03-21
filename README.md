# Travel Brochures

Interactive trip brochures hosted via GitOps on NAS.

## Structure
```
/
├── index.html                    # Landing page listing all trips
├── research/
│   └── [trip-slug]/
│       └── index.html            # Individual trip brochure
└── README.md
```

## Deployment
- **GitHub repo:** `lamarbot-ai/travel-brochures`
- **NAS path:** `/volume1/home-lab/travel-brochures/`
- **Container:** `travel-brochures` (nginx + git-sync)
- **Public URL:** `https://travelplanning.lamaroliphant.com/`

## Adding a New Trip
1. Create folder: `research/[trip-slug]/`
2. Add `index.html` with the brochure
3. Update root `index.html` with new card
4. Commit and push - auto-deploys in ~60s

## URL Format
```
https://travelplanning.lamaroliphant.com/research/[trip-slug]/
```
