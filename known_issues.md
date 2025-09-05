# Known issues

## With v2.2.3
1. Charts not shown: clash with older versions of apexcharts.js used in HA
2.2.x introduced an updated (external) library apexcharts.js which has shown to have issues with other HA elements
- edata
- verhicle card
- possibly other

Check in the open and (!) closed issues for possible workarounds

2. Graphs cut-off
2.2.3 increased support for functionality in dashboard/view with Sections, but also shown challenges
- horizontal stack
- possibly other
Experiment with the new (!) config parameter ```section_mode``` https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#main-options

Check in the open and (!) closed issues for possible workarounds
