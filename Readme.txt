
# GpstoExcel

## Description
This script extracts GPS metadata from images and saves the information into an Excel file. It utilizes the PIL (Pillow) library to handle image processing and OpenPyXL for Excel file creation.

## Prerequisites
- Python 3.x

## Installation
1. Ensure Python 3 is installed on your machine.
2. Install the required Python packages using the provided `requirements.txt` file:
   ```
   pip install -r requirements.txt
   ```

## Usage
1. Place your images in a directory.
2. Update the `image_directory` variable in the script to point to your image directory.
3. Run the script:
   ```
   python GpstoExcel.py
   ```
4. The script will generate an Excel file named `output.xlsx` with the extracted GPS data.

## Script Details
- `get_exif_data(image_path)`: Extracts EXIF data from the given image.
- `get_gps_info(exif_data)`: Extracts GPS information from the EXIF data.
- `convert_to_degress(value)`: Converts GPS coordinates from degrees, minutes, and seconds to decimal degrees.
- `get_lat_lon(gps_info)`: Retrieves latitude and longitude from GPS information.

## Example
1. Ensure your images are in the specified directory.
2. Run the script.
3. Check the generated `output.xlsx` file for GPS metadata.

## Dependencies
- PIL (Pillow)
- openpyxl
- fractions

## License
This project is licensed under the MIT License - see the LICENSE file for details.
