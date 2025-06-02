Spatial Analysis with ArcGIS - ENGR 180 📍

This repository contains course materials, labs, and final project for ENGR 180: Spatial Analysis with ArcGIS. The course covers fundamental concepts and practical applications of spatial analysis using Esri's ArcGIS platform.

Repository Structure
📂 Grand Final Project: ADA Compliance Project (20+ pages)
ADA Industrialization Project At Yosemite National Park_HaoDinhMai_July 1, 2022FinalReport.pdf - Comprehensive report on ADA compliance at Yosemite

Datafest Report_HaoDMai.pdf - Data analysis project report

ENGR 180 Summer DataFest Presentation_May 25, 2022_HaoDinhMai.pptx - Presentation slides

Instruction.pdf - Project guidelines and requirements

🔬 Labs
Lab 01: Spatial Reference & Projection
CaseStudy1-1.pdf - Case study document

Engr180_Lab01_CaseStudy1-1_HaoDMai_6.2.22.pdf - Lab report

Lab 01-2: Buffer & Contrast
Case Study 1-2_Identifying Threats of Contamination to Merced County Rivers.pdf - Analysis report

CaseStudy1-2.pdf - Case study document

Lab 02-1: ModelBuilder
CaseStudy2-1.html - Interactive case study

Lab2-1_Hao Mai_6.9.22.pdf - Lab report

Lab 02-2: Python with ArcGIS
CaseStudy2-2.html - Interactive case study

Hao Dinh Mai_Engr_Case2-2_6.14.22-1.pdf - Lab report

Lab 03: Rasters & Cells
casestudy3-rasters.html - Interactive raster analysis

Hao Dinh Mai_CaseStudy3_Lab4a_6.16.22.pdf - Lab report

Lab 04: Raster Function
Hao D Mai_CaseStudy4_May 20, 2022.pdf - Lab report

Lab 05: Spatial Interpolation
casestudy5.html - Interactive spatial interpolation

Hao D Mai_CaseStudy5_May 25, 2022.pdf - Lab report

🛠 Technical Requirements
ArcGIS Pro 3.x or ArcMap 10.8+

Python 3.x with ArcPy library

Spatial Analyst extension

3D Analyst extension (for some labs)

📚 Course Concepts Covered
Spatial reference systems and map projections

Geoprocessing workflows

Spatial data modeling

Raster analysis and processing

Spatial interpolation techniques

Python automation for GIS

Cartographic design principles

🗺 Sample Project Preview
python
# Sample ArcPy script for spatial analysis
import arcpy
from arcpy.sa import *

# Set environment settings
arcpy.env.workspace = "C:/data/Yosemite"
arcpy.env.overwriteOutput = True

# Perform accessibility analysis
in_features = "trails.shp"
buffer_distance = "1000 feet"
out_buffer = "accessible_areas.shp"

# Create buffer around ADA accessible trails
arcpy.Buffer_analysis(in_features, out_buffer, buffer_distance)

# Calculate accessible area statistics
result = arcpy.GetCount_management(out_buffer)
print(f"Created {result[0]} accessible areas")
📊 Key Projects
ADA Compliance Analysis at Yosemite National Park

Accessibility mapping

Facility suitability analysis

Compliance gap identification

Merced County Water Contamination Risk Assessment

Watershed delineation

Contaminant dispersion modeling

Risk zone classification
