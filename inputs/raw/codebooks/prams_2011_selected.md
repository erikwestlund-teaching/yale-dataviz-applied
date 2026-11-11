# PRAMS 2011 Selected Data Codebook

File: `inputs/raw/prams_2011_selected.csv`

Source: CDC PRAMStat 2011 public data, processed from the previous course materials.

Rows: 1,222

Columns: 8

## Unit Of Observation

Each row is a pre-aggregated percentage for one location, subgroup category, and subgroup.

Values are percentages reported by PRAMS for specific state and subgroup combinations. They are not person-level records.

## Variables

- `location_abbr`: State or location abbreviation.
- `location`: Full state or location name.
- `subgroup_cat`: Subgroup category, such as maternal age, marital status, income, or number of previous live births.
- `subgroup`: Specific subgroup within `subgroup_cat`.
- `depression_within_3_months_birth`: Percent who had depression during the 3 months before pregnancy. PRAMS question: "During the 3 months before you got pregnant with your new baby, did you have depression?" (PRAMStat QUO133).
- `anxiety_within_3_months_birth`: Percent who had anxiety during the 3 months before pregnancy. PRAMS question: "During the 3 months before you got pregnant with your new baby, did you have anxiety?" (PRAMStat QUO232).
- `binge_drinking_within_3_months_birth`: Percent who binge drank (4 or more drinks) during the 3 months before pregnancy (PRAMStat QUO271).
- `alcohol_use_within_3_months_birth`: Percent who drank any alcohol during the 3 months before pregnancy (PRAMStat QUO8).

The column names say "birth", but all four measures refer to the 3 months before pregnancy. PRAMStat definitions: <https://data.cdc.gov/d/ese6-rqpq>.

## Teaching Notes

- This dataset suits grouped bar charts, facets, ranks, missingness, and the interpretation of pre-aggregated data.
- Depression and anxiety measures have substantial missingness.
- Students should always state the subgroup and location structure when interpreting a plot.
