# Known issues

## With v2.2.3
1. Charts not shown: 
2.2.x introduced an updated (external) library apexcharts.js which has shown to clash with older versions of apexcharts.js used in other elements of HA
- edata
- verhicle card
- possibly other(?)

Check in the open and (!) closed issues for possible workarounds.
**This apexchard-card repo will not pursue/request changes of other integrations/cards**

== ref. ===

Until the edata integration is updated by its author, you might be able to manually edit the file /custom_components/edata/www/edata-card.js and replace
import "https://cdnjs.cloudflare.com/ajax/libs/apexcharts/3.45.1/apexcharts.min.js?module";
with
import "https://cdnjs.cloudflare.com/ajax/libs/apexcharts/5.3.3/apexcharts.min.js?module";

== end ref. ===

Similar may work for the vehicle-info card.

2. Graphs cut-off
2.2.3 increased support for functionality in dashboard/view with Sections, but also shown challenges
- horizontal stack
- possibly other
Experiment with the new (!) config parameter ```section_mode``` https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#main-options

Check in the open and (!) closed issues for possible workarounds
