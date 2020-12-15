### REQUIRED DATA CITATION:

U.S. Department of Transportation, Research and Innovative Technology Administration, Bureau of Transportation Statistics, Freight Transportation: T-100 Domestic Market (U.S. Carriers), 2020 (Washington, DC: 2020)

U.S. Department of Transportation, Research and Innovative Technology Administration, Bureau of Transportation Statistics, Freight Transportation: T-100 International Market (All Carriers), 2020 (Washington, DC: 2020)

All material contained in this report is in the public domain and may be used and reprinted without special permission; citation as to source is required.

### Air travel metadata:

#### Column Headers:

- timestamp: ISO-8601. Flight data is aggregated to months

- origin_airport_code: Three letter airport identifier code (string)

- origin_city: long-form name of departure city (string)

- origin_state_abr: Two letter abbreviation of departure city (string)

- origin_admin2: US-only, State of departure airport (string)

- origin_fips: US-only, 5-digit county FIPS code of the departure airport (string)

- origin_admin1: State or Province of departure airport (not all non-US airports mapp to an admin1) (string)

- origin_admin0: Country of departure airport (string)

- origin_iso2: Two-letter country code of departure airport in ISO 3166-1 alpha-2 standard (string)

- dest_airport_code: Three letter airport identifier code (string)

- dest_city: long-form name of arrival city (string)

- dest_state_abr: Two letter abbreviation of arrival city in ISO 3166-1 alpha-2 standard (string)

- dest_admin2: US-only, State of arrival airport (string)

- dest_fips: US-only, 5-digit county FIPS code of the arrival airport (string)

- dest_admin1: State or Province of departure airport (not all non-US airports mapp to an admin1) (string)

- dest_admin0: Country of arrival airport (string)

- dest_iso2: Two-letter country code of arrival airport (string)

- distance: Distance in miles from departure to arrival airport (float)

- passengers: number of passengers travelling from departure to arrival airport; does not include layover passenger data. (int)
For example: if you fly from CLE to PDX with a layover in DEN, you are only counted once for the CLE to PDX flight. 
For further explanation see: https://transportation.libanswers.com/faq/166158
