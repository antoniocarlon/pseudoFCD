##Pseudo Forest Canopy Density (pseudo-FCD)

**Pseudo Forest Canopy Density** is a script for the **Sentinel-hub EO-Browser** (https://apps.sentinel-hub.com/eo-browser) that classifies each pixel of the satellite images into one of the following categories:
 * High Forest
 * Low Forest
 * Grassland
 * Bare land
 * Water
 * Unknown

This allows the user to explore forest zones to fight deforestation, for agricultural purposes and even for city planning.

According to the reference, the Forest Canopy Density (FCD) is calculated using four different indices:
 * Advanced vegetation index (AVI)
 * Bare soil index (BI)
 * Canopy shadow index (SI)
 * Thermal index

The script (and hence the name) implements a custom version of the AVI, BI and SI indices and uses the Table 3 shown in the reference along with experimental threesholds to make the classification. It can be used with **Sentinel-2 L1C and L2A**.

As the main drawback, the script has problems with some water bodies.

Althought the default threesholds for each category work quite good for most of the situations, they can be tweaked depending on the location to fine tune the results. The script can also be configured to avoid detecting water bodies.

#### Examples

![Image 1](/images/Image1.png)
![Image 2](/images/Image2.png)
![Image 3](/images/Image3.png)
![Image 4](/images/Image4.png)

#### References

[1] Azadeh ABDOLLAHNEJAD*, Dimitrios PANAGIOTIDIS, Peter SUROVÝ. "Forest canopy density assessment using different approaches – Review". Journal of Forest Science, 63, 2017 (3): 106–115. https://www.agriculturejournals.cz/publicFiles/210529.pdf