# Electric Vehicle Population Analysis Dashboard

# Overview

This project analyzes the Electric Vehicle (EV) population in the United States using the Electric_Vehicle_Population_Data.csv dataset. As a data analyst, I cleaned and prepared the dataset, developed an interactive Tableau dashboard to visualize key trends, and derived actionable insights on EV adoption, model popularity, and eligibility for Clean Alternative Fuel Vehicle (CAFV) incentives. The dashboard highlights distributions by state, model, and electric vehicle type, showcasing my expertise in data cleaning, visualization, and analytical storytelling.

# Dataset

The original dataset, Electric_Vehicle_Population_Data.csv, contains 150,482 records with the following fields:

VIN (1-10): Vehicle Identification Number (string, 9,893 unique values)

County, City, State: Geographic location (string, 69 counties, 767 cities, 61 states)

Postal Code, Model Year: Vehicle details (integer, 983 postal codes, 14 model years from 2011 to 2024)

Make, Model: Manufacturer and model (string, 54 makes, 342 models like MODEL Y, MODEL 3, LEAF)

Electric Vehicle Type: Type of EV (string, 2 types: Battery Electric Vehicle (BEV), Plug-in Hybrid Electric Vehicle (PHEV))

Clean Alternative Fuel Vehicle (CAFV) Eligibility: Eligibility status (string, 3 categories: Eligible, Not Eligible, Unknown)

Electric Range, Base MSRP: Range and price (integer, 215 range values, 99 MSRP values)

Legislative District, DOL Vehicle ID, 2020 Census Tract: Additional identifiers (integer)

Vehicle Location, Electric Utility: Location and utility provider (string, 983 locations, 109 utilities)

The dataset provides a comprehensive view of EV adoption across the U.S. from 2011 to 2024.

# Dashboard Creation in Tableau

 Key Visualizations:

Total Vehicles by State: A U.S. map displaying the count of EVs by state, with California (92 vehicles) and Washington (8 vehicles) leading adoption.

Total Vehicles Model Year: A line chart showing EV growth from 2011 (796 vehicles) to 2024 (11,294 vehicles), with an average of 10,744 vehicles per year.

Top Vehicles by Make: A bar chart highlighting top manufacturers (e.g., TESLA with 69,939 vehicles, 46.34% of total).

Top Vehicles by CAFV Eligibility: A pie chart breaking down eligibility (46.34% Eligible, 41.81% Not Eligible, 11.85% Unknown).

Top Vehicles by Model: A table listing popular models (e.g., MODEL Y with 28,501 vehicles, 18.92% of total).

EV Type Summary: KPIs showing total BEV vehicles (116,745, 78%) and total PHEV vehicles (33,668, 22%), with an average electric range of 116,745 miles.

Calculated Fields:

Total BEV vehicles: SUM(IF [Electric Vehicle Type] = "Battery Electric Vehicle (BEV)" THEN 1 ELSE 0 END)

%of total: SUM(IF [Electric Vehicle Type] = "Battery Electric Vehicle (BEV)" THEN 1 ELSE 0 END) / COUNT([VIN (1-10)])

Filters and Interactivity:

Added filters for State, Model, Electric Vehicle Type, Clean (CAFV) Eligibility, and Model Year (2011–2024 slider) to allow dynamic exploration.

Design:


Used a clean layout with a light background, green accents for readability, and tooltips for detailed data on hover.

The dashboard provides an interactive view of EV population trends and eligibility metrics.

# Key Insights

Adoption Trends: California and Washington lead with 92 and 8 vehicles, respectively, indicating regional hotspots for EV adoption.

Growth Over Time: EV registrations have grown significantly, from 796 in 2011 to 11,294 in 2024, reflecting increasing market penetration.

Manufacturer Dominance: TESLA dominates with 69,939 vehicles (46.34%), showcasing strong brand loyalty.

EV Type Distribution: BEVs account for 78% of the population (116,745 vehicles), suggesting a preference for fully electric vehicles.

CAFV Eligibility: 46.34% of vehicles are CAFV-eligible, while 41.81% are not eligible due to low battery range, and 11.85% are unknown, indicating a data gap.

Popular Models: MODEL Y leads with 28,501 vehicles (18.92%), followed by MODEL 3 (18,861) and LEAF (27,798), highlighting consumer preferences.

These insights demonstrate my ability to extract meaningful patterns from complex datasets and present them effectively.
