# Brawl Stars Tier List Dataset

This dataset contains Brawl Stars brawler tier lists collected from various content creators.

## Format

The dataset is stored in `data.json` with the following structure:

```json
[
    {
        "handle": "...",
        "link": "https://www.youtube.com/@...",
        "totallyOrdered": "...",
        "tierLists": [
            {
                "date": "DD/MM/YYYY",
                "link": "https://youtu.be/...",
                "list": [
                    ["Brawler 1", "Brawler 2", "..."],
                    ["Brawler 3", "Brawler 4", "..."]
                ]
            }
        ]
    }
]
```

### Field Descriptions

- **`handle`** — The YouTube handle of the creator.  
- **`link`** — The URL to the creator's YouTube channel.  
- **`totallyOrdered`** — Indicates whether the tier lists are sorted from best to worst (`true` or `false`)<sup>[1]</sup>.  

Each entry in the `tierLists` array includes:

- **`date`** — The date the tier list video was posted, formatted as `DD/MM/YYYY`.  
- **`link`** — A shortened `youtu.be` link to the tier list video.  
- **`list`** — The tier list itself, where each nested array represents a tier, sorted from best tier to worst.  

## Notes

1. The first brawler in the first tier is the best, the last brawler in the last tier is the worst.
