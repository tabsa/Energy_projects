# Electric vehicle charging analysis

## Overview

The `ev_charger_analysis` module is designed to decode raw data from Electric Vehicle (EV) chargers and transform it into a more structured format for analysis. This module provides functionality to decode raw data stored in text (txt) or comma-separated values (csv) format and digest it into Pandas DataFrames.

### Folder Structure

The module has the following folder structure:
- **decoder/**: Contains code related to decoding raw data.
  - `decoder.py`: Implements the decoding functionality to separate raw data into dictionaries for further processing.

- **digestor/**: Contains code related to digesting dictionaries into DataFrames.
  - `digestor.py`: Implements the functionality to digest dictionaries into Pandas DataFrames with augmented data for human readability.

## Usage

To use this module, follow these steps:

1. Install the module using pip:

   ```bash
   pip install ev_charger_analysis
   ```

## Example
  ```
  from ev_charger_analysis.decoder import decode_raw_data
  from ev_charger_analysis.digestor import digest_data_to_dataframe
  
  from ev_charger_analysis.decoder import decode_raw_data
  from ev_charger_analysis.digestor import digest_data_to_dataframe
  
  # Step 1: Decode raw data
  raw_data = "Your raw data here"
  decoded_data = decode_raw_data(raw_data)
  
  # Step 2: Digest decoded data into DataFrame
  df = digest_data_to_dataframe(decoded_data)
  
  # Now you can analyze the DataFrame as needed
  print(df.head())
  ```

# Contribution
Contributions to this module are welcome! If you find any bugs or have suggestions for improvement, please feel free to open an issue or create a pull request on GitHub.

# License
Feel free to customize it further based on your specific needs or additional information you want to include!
