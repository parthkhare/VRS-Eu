---
title: Nightlights: Products and intrinsic limitations
description: Translating remote sensing for researchers
toc: true
authors:
  - Example Author
tags:
  - image
categories:
  - themes
series:
  - Themes Guide
date: '2020-05-26'
lastmod: '2020-05-26'
featuredImage: images/NTLgridtiles.png
draft: false
---

Raw Nightlights data is available in raster imagery at NOAA, EOD, where the world is split into 6 tiles

<!--more-->


## Defense Meteorological Satellite Program (DMSP) - Annually 1992-2012

US Air Force Defense Meteorological Satellite Program (DMSP) Operational Linescan System (OLS) was launched in 1992. Satellites from the United States Air Force Defense Meteorological Satellite Program (DMSP) circle the earth 14 times per day. They record the intensity of Earth-based lights with their Operational Linescan System (OLS) sensors since the 1970s, with a digital archive beginning in 1992. These sensors were designed to collect low-light imaging data for the purpose of detecting moonlit clouds, but a byproduct is that lights from human settlements are recorded. Each satellite observes every location on the planet every night at some instant between 8:30 and 10:00 pm local time. National Oceanic and Atmospheric Administration’s (NOAA) National Geophysical Data Center (NGDC) processes this data by removing observations for places experiencing the bright half of the lunar cycle, the summer months when the sun sets late, auroral activity (the northern and southern lights),and forest fires. Observations where cloud cover obscures the earth’s surface are also excluded. These restrictions remove intense sources of natural light, leaving mostly man-made light. Finally, data from all orbits of a given satellite in a given year are averaged over all valid nights to produce a satellite-year dataset.

As suggested by the name its intended purpose was to detect surface objects (moving tanks, ships) 
from the sky, with an arguable application during Desert Fox. Later it was released for public access by NOAA, and has since then being used as a proxy for economic activity, particularly for regions with poor statistical capacity. Despite its unqiue ability to glean economic activity based on radiance intensity on ground, it still suffered from a couple of issues, namely:
- Scale limitation: DMSP sensor can measure light intensity between 0 to 63 only, due to 6-bit radiometric resolution or quantization
- Top Coding: As a consequence of range, low and highly lit areas often show same values (mode=37) due to pixel-value saturation in bright urban core areas. This obfuscates nightlight details within brightly lit areas such as cities and towns, limiting it's ability to discern between unplanned slums and affluent areas within a city.
- Sensor degradation: Sensors onboard the DMSP satellites would degrade over time adversely affecting their accuracy over time. This was partially addressed by fitting multiple sensors (F12-F15) and making use of the overlapping years to calibrate. However, it was still difficult for non remote sensing experts to calibrate across sensors.
_ Biophysical/Seaonal Noise


DMSP Unit: Digital Number (DN) is a ratio of Upwelling and Downwelling Radiance therefore it is a unitless ratio measuring net reflectance

## Visible Infrared Imaging Radiometer Suite (VIIRS) - Monthly/Annually 2012- 

Visible Infrared Imaging Radiometer Suite (VIIRS) on-board the SUOMI-NPP satellite, replaced the US Air Force Defense Meteorological Satellite Program (DMSP) Operational Linescan System (OLS)-based data since 2012. The VIIRS is available from the United States National Oceanographic and Atmospheric Administration (NOAA) at a monthly frequency starting from April 2012. In addition, NOAA provides two annual images (recently released from 2012 to 2020: v20) which removes several artifacts from the raw series. 

VIIRS Day/Night Band (DNB) on-board the SUOMI-NPP satellite has a finer ground footprint of 742 x 742 m, a radiometric resolution of 14-bit (addressing pixel saturation problem), a low light detection limit that allows detecting lights from dimly-lit human settlements such as from rural areas. As a result, NTL data derived from the VIIRS DNB provides a high resolution and consistent time-series dataset to monitor artificial or man-made sources of lights. However, it still suffers from biophysical noises including cloud cover. This particularly affects the monthly product which


VIIRS Unit: DNB Radaiance captures radiance measured in watts/cm2/sterdians
multiplying the pixel value by 10^9 gives radiance in units of W/cm2-sr 

## Cleaning

