# ASMR Registry catalog data

Summary statistics about YouTube ASMR videos, from the [ASMR Registry](https://asmrregistry.com/) catalog. Snapshot: 2026-11-08.

## Files

| File | What it holds |
|---|---|
| `asmr-trigger-stats.csv` | For each main ASMR trigger with 30 or more videos: video count, median length in minutes, share of videos 30 minutes or longer, share labelled "no talking". |
| `asmr-trends-by-year.csv` | For each upload year with 300 or more videos: video count, median length, share over one hour, share labelled "no talking", share in Korean, and the shares of eating sounds, whispering and tapping. |

Live versions, updated with each site build: [ASMR statistics](https://asmrregistry.com/guides/asmr-statistics/) and [ASMR trends by year](https://asmrregistry.com/guides/asmr-trends/).

## How the data was made

- The catalog collects popular, findable ASMR videos from YouTube through the YouTube Data API. Older years hold only videos that stayed popular and online, so the data shows what is watched and still available, not every upload.
- Each video's main trigger, "no talking" label and language are assigned by an AI model from the video's title and description. Nobody listens to the videos, so some labels are wrong.
- Lengths come from YouTube. Every stored video is rechecked against YouTube at least every 30 days.
- The files contain only counts and shares we computed. They contain no video titles, IDs, view counts or other YouTube data.

Method in more detail: https://asmrregistry.com/methodology/

## Licence and credit

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit "ASMR Registry (asmrregistry.com)" and, where possible, the DOI shown on the Zenodo record.
