# CAM-EIA

## Plan
Things we need to d3.js and ember.js to interactively separate data into these views. 

* Pick a timescale: Annual/Quarterly/Monthly 
    * Pick a year/quarter/month, ie, 2012/2014Q3/201602
    * ALT: implement a slider for time
        * e.g., Annual goes through all the data
* Show All US
    * or, Pick a location out of (51 states + 10 Regions + 1 All US): 
        * All US
            * Any of 51 states: AK/AL/etc.
        * Region: ENC/ESC/MAT/MTN/NEW/PCC/PCN/SAT/WNC/WSC
* Show all sources: fossil fuels/nuclear/hydro/biomass/other renewables/other
    * or, pick one source and separate into subsources, see section below.

Notes. Missing data will be marked as 0. Units are in thousand megawatthours, i.e. GWhr. There are 50 states + DC.

## Appendix: Fuel Types/Sources and Subsources

See eia_tech_notes.pdf pg14 for more, but not all, of the abbreviations. Unconfirmed abbv.: (PEL) (COW) (WWW) (WAS) (AOR) (OOG).

* "1": "all fuels" (ALL)
    * (fossil fuels)
        * "4": "coal"
        * "7": "petroleum liquids"
        * "8": "petroleum coke"
        * "9": "natural gas" (NG)
        * "10": "other gases"
    * (nuclear) (NUC)
        * "11": "nuclear"
    * (hydro)
        * "12": "conventional hydroelectric" (HYC)
        * "19": "hydro-electric pumped storage"
    * (biomass)
        * "16": "wood and wood-derived fuels"
        * "18": "other biomass"
    * (other renewables)
        * "13": "other renewables (total)"
            * (wind) (WND)
                * "14": "wind"
            * (solar) (SUN)
                * "1718408": "all solar"
                    * "15": "all utility-scale solar"
                        * "1718400": "utility-scale photovoltaic"
                        * "1718401": "utility-scale thermal"
                    * "1718409": "distributed solar"
            * (geothermal) (GEO)
                * "17": "geothermal"
    * (other) (OTH)
        * "20": "other"
