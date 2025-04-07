 `Title`: HOLC grades from the Mapping Inequality Database (MID)
- `Abstract`: HOLC grades are historical neighborhood delineations created by the Home Owners’ Loan Corporation in the 1930s to assess mortgage lending risk. These maps were used to guide investment and disinvestment in urban areas
 and are a foundational dataset for understanding redlining and its long-term impacts.
- `Spatial Coverage`: Select major U.S. cities
- `Spatial Resolution`: Neighborhood-scale boundaries (city block to district level, variable by city)
- `Spatial Representation Type`: `vector`, `MULTIPOLYGON`
- `Spatial Reference System`: `NAD83`
- `Temporal Coverage`: 1935–1940 (approximate dates of HOLC map creation)
- `Temporal Resolution`: Single mapping effort. 
- `Lineage`: Downloaded and used as-is.
- `Distribution`: Data is publically avalible from the Mapping Inequality website (https://dsl.richmond.edu/panorama/redlining/data)[https://dsl.richmond.edu/panorama/redlining/data]
- `Constraints`: Publically avalible data.
- `Data Quality`: Accurate to the degree that the original digitization of the 1930's HOLC maps was accurate. 

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| city | City Name | City in which the HOLC designated area resides | character | N/A | Names of US cities | none | none |
| state | State Abbreviation | USPS state designator | character | N/A | The 50 states | N/A | none |
| category | Desirability | Assessment of investment desirability based on HOLC designation  | character | subjective/historical | a range of desigations | none | none |
| grade | Grade | Historical HOLC grade | character | subjective/historical | A - D | none | none |
| label | Shape Label | HOLC grade and arbitrary number (A1, C3) to divide same-grade areas from the same city| character | N/A | A-D, number of same-grade zones in the same city | none | none |
| residential | Is it residential? | " " | bianary (TRUE/FALSE) | N/A | TRUE/FALSE | none | none |
| commercial | Is it commercial? | " "  | bianary (TRUE/FALSE) | N/A | TRUE/FALSE | none | none |
| industrial | Is it industrial? | " "  | bianary (TRUE/FALSE) | N/A | TRUE/FALSE | none | none |
