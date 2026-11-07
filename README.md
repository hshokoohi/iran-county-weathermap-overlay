# iran-county-weathermap-overlay
Python/Jupyter tool that overlays Persian county names, county-seat locations, administrative boundaries, coastlines, and map annotations onto Meteologix weather-forecast maps using GIS data. Configured with a Bushehr Province preset; exports high-resolution PNG/PDF.

# README intro
This notebook is designed to add county names and county-seat locations for Bushehr Province — and, more generally, Iran — to raw weather-model output maps from Meteologix. It georeferences the input map, loads official county lists and GIS boundary/coastline data, and places Persian labels without covering the model’s contour numbers or maximum values. It is intended for producing clear, publication-quality localized forecast maps.

# Key features
Adds Persian county names and county-seat locations to Meteologix forecast maps.
Uses GIS data for county, province, and international boundaries; coastlines; and islands.
Places county names inside county polygons, with slanted labels along the county’s long axis when useful.
Avoids collisions with boundaries, other labels, and the model’s own numbers.
Shows province capitals with a star and a highlighted name.
Adds sea, strait, neighbouring-country, and island names.
Preserves the original model map values during high-resolution upscaling.
Includes a Persian header with forecast period in the Jalali calendar and Iran time.
Exports high-resolution PNG and PDF with vector labels and lines.
Includes a ready-to-use Bushehr Province preset.

# Data sources
* Official Iranian county/city list: sajaddp/list-of-cities-in-Iran
* Administrative boundaries: geoBoundaries IRN ADM1/ADM2
* Coastlines and international borders: Natural Earth 1:10m
OSM-derived coastal detail for Bushehr Province
Persian font: B Yekan, with Vazirmatn fallback
