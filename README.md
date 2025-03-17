# Brawl Stars Tier List Dataset

A dataset containing Brawl Stars brawler tier lists collected from various creators.

## Format

The dataset is stored in `data.json` with the following structure:

```json
{
    "creator_name": [
        {
            "date": "DD/MM/YYYY",
            "link": "https://youtu.be/...",
            "list": [
                ["Brawler 1", "Brawler 2", ...],
                ["Brawler 3", "Brawler 4", ...]
            ]
        }
    ]
}
```

**`creator_name`** — The YouTube handle of the creator.  
**`date`** — The date the video was posted, in `DD/MM/YYYY` format.  
**`link`** — The shortened `youtu.be` link to the tier list video.  
**`list`** — The tier list itself, with each nested array representing a tier, sorted from best to worst.

## Notes

- Kairos sorts his brawlers from best to worst: the first brawler in the first tier is the best and the last brawler in the final tier is the worst.
