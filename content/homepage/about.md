---
title: Nightlights for Economic Development 
draft: false
role: Parth Khare
avatar: images/IndiaNL.png
bio: Shedding lights on nightlights:DMSP-VIIRS-Black Marble 
organization:
  name: CGD
  url: https://www.cgdev.org/
social:
  - icon: envelope
    iconPack: fas
    url: mailto:parthakhare@gmail.com
  - icon: twitter
    iconPack: fab
    url: https://twitter.com/parthakhare/
  - icon: github
    iconPack: fab
    url: https://parthkhare.github.io/

weight: 1
widget:
  handler: about

  # Options: sm, md, lg and xl. Default is md.
  width:

  sidebar:
    # Options: left and right. Leave blank to hide.
    position:
    # Options: sm, md, lg and xl. Default is md.
    scale:
  
  background:
    # Options: primary, secondary, tertiary or any valid color value. Default is primary.
    color: secondary
    image:
    # Options: auto, cover and contain. Default is auto.
    size:
    # Options: center, top, right, bottom, left.
    position:
    # Options: fixed, local, scroll.
    attachment: 
---

## Nightlights as a proxy for economic growth

#### Story so far: DMSP 1992-2012
Nighttime lights or nightlights have been used as a proxy of economic activity as lights emanating from residential settlements and commercial establishments contain signatures of human activity. After the seminal work by [Henderson Weil Storeygard](https://www.aeaweb.org/articles?id=10.1257/aer.102.2.994) in 2012, establishing relation nighlights (DMSP) and economic growth rate, several others studies have further explored the said association at macro levels (estimating GDP for poorer countries) and for micro interventions (proxying economic activity at high resolution i.e. villages through nightlights). In other words, nightlights has been used a proxy for either assessing growth for countries with lagged, incredulous census data or a correlate of growth while testing efficacy of interventions at a micro level.

 
#### Better data but fewer studies: VIIRS/Black Marble 2012- 
Despite its success as a useful proxy, The Defense Meteorological Satellite Program— Operational Linescan System or DMSP-OLS satellite faced multiple problems, including sensor degradation and [top coding](https://onlinelibrary.wiley.com/doi/abs/10.1111/obes.12417). In addition, the DMSP program had to frequently re launch different sensors (F12, F13,F14) periodically. In an attempt to improve these infirmities, a better product suite called Visible Infrared Imaging Radiometer Suite (VIIRS) on board the SUOMI-NPP satellite was released. It addressed many of the drawbacks inherent within DMSP. However, despite being a better data source, VIIRS has proved challenging to explain economic activity at a country level so far. Moreover, a cleaner version of the VIIRS data (addressing cloud cover, noisy pixels) was later re-released by NASA in 2021/2022, called BlackMarble.

Tldr: VIIRS or Blackmable do not explain country level growth at least much as DMSP explained. However, despite this many localized  studies still exploit this association by using VIIRS as a proxy for measuring effectiveness of various development interventions. Why is it that despite improved data, is there an attenutation in the association between nightlights-economic growth, or were measuring it wrong all along? 





## Anlysis Framework: New Nightlights (VIIRS & BlackMarble)

Following work is a near-exhaustive compilation of testing the efficacy and potential of VIIRS and Black Marble, the analysis is categorized in different levels:
- Low pass: NL explaining economic events (wars, calamities, covid)
- Mid pass: NL explaining localised growth 
- High pass: NL explaining global growth

Along with testing these hypotheses, we also look for limited scenarios regions where this data works, and explore deeper reasons for why in the said associations fail despite improved data.



### Index
- [Global trends](https://nightlights-econ.netlify.app/posts/2021-10-14-global-trends/)
- [Regressions-Attenuation](https://nightlights-econ.netlify.app/posts/2020-12-01-r-rmarkdown/)
  - HWS, Goldberg
  - Overlap  
  - HMC/LMC
- [Covid](https://nightlights-econ.netlify.app/posts/2021-10-15-covid-ntl/)
- [Cleaning nightlights](https://nightlights-econ.netlify.app/posts/2021-10-14-cleaning-variants/)
  - Variant creation, Addressing negative values
- Scale: micro vs macro
- Different specifications ?
- Appendix research (Colombia, LULC)

## About Nightlights
- [Products (DMSP-VIIRS)](https://nightlights-econ.netlify.app/posts/featured-image/) 
- [Literature](https://nightlights-econ.netlify.app/posts/2021-10-15-litrev/)



## Caveat thinking: On Macroecnomics and Big Data (Signal/Noise)
One of the central goals of macroeconomics is to explore and build associations which stand test of time and can be established as natural laws. From 101's of interest rate and inflation or employment and monetary policies, building such fundamentals and translating them as models help in cleaning signal from noise by synthesizing information/data along existing models. 

One of the main resaons why big or high frequency data still struggles to breakthrough in this realm (third wave economics et al), is because extracting signal from such dense and high volumed dataset is challenging, given the relative proportion of noise. Either the high frequency data should explain existing models or alternatively there should be a different set of models that need to be looked into for understanding such phenomenons. Motivated by this the 

