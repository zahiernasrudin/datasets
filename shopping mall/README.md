# Shopping Mall list in Malaysia

## Overview

This dataset lists all the shopping malls available in Malaysia. It contains information about shopping malls, including their names, locations, and status. It is sourced from multiple websites and the Google API for geolocation.

## Dataset Details

-   Extracted on October 1 2024

-   The dataset contains **219 rows** & **8 columns**

| **Column Name**     | **Data Type** | **Description**                                                                                                      | **Example**                                                                                             |
|--------------|--------------|-------------------------------|--------------|
| `name`              | Text          | Name of the shopping mall.                                                                                           | "Pavilion Kuala Lumpur"                                                                                 |
| `lat`               | Numeric       | Latitude of the shopping mall's location, based on geolocation data.                                                 | 3.1489607                                                                                               |
| `lng`               | Numeric       | Longitude of the shopping mall's location, based on geolocation data.                                                | 101.7134125                                                                                             |
| `place_id`          | Text          | Unique identifier for the mall's location from the Google API.                                                       | "ChIJm1A1iSw2zDERtJ-nsFBslu0"                                                                           |
| `formatted_address` | Text          | Full address of the shopping mall, formatted for clarity (from Google API).                                          | "168, Jln Bukit Bintang, Bukit Bintang, 55100 Kuala Lumpur, Wilayah Persekutuan Kuala Lumpur, Malaysia" |
| `state`             | Text          | The state in which the shopping mall is located, based on the boundaries set by the government.                      | "W.P. Kuala Lumpur"                                                                                     |
| `district`          | Text          | The district within the state where the shopping mall is situated, based on the boundaries set by the government.    | "W.P. Kuala Lumpur"                                                                                     |
| `status`            | Text          | Operational status of the mall ("Operational", "Closed", "Coming soon", "Temporarily closed", "Permanently closed"). | "Operational"                                                                                           |

## **Data Cleaning Steps**

1.  **Webscraping**
    1.  Data was collected from multiple available websites
2.  **Geolocation Processing**
    1.  Used the Google API to retrieve precise latitude and longitude for each mall based on its address.
3.  **Mapping State and District**
    1.  Utilized government data to map each shopping mall to the correct state and district. (Based on the latitude & longitude information)

## Contact

For any inquiries or further information, please contact me. As this is an open-source dataset, feel free to contribute or provide feedback regarding any missing or incorrect information.
