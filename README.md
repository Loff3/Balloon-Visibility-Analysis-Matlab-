  # Balloon Visibility Analysis

  Identifierar optimal placering och höjd för en reklamballong för maximal synlighet från gångbara ytor i centrala Gävle genom 3D-viewshedanalys.
  
![Vy 1](2026-04-29_15-45-32.png)

  ## Mål
  - Maximera synlighet från gångbar mark.
  - Jämföra synlighet mellan olika positioner, höjder och riktningar.
  - Bygga interaktiva visualiseringar för beslutstöd.

  ## Data
  - `Gavle_025_5000.tif` (DSM)
  - `Mask_025_5000.png` (gångbarhetsmask)
  - Nersampling: 0.25 m -> 0.5 m (5000x5000 -> 2500x2500)

  ## Metod
  1. Förbehandling och nersampling av DSM + mask.
  2. 3D-skalärfält: relativ synlighet per punkt i volymen.
  3. 3D-vektorfält: riktning för maximal synlighet (36 azimutriktningar per punkt).
  4. Optimering av beräkning med `parfor`.
  5. Geovisualisering med iso-ytor, slicing och vektorpilar.

  ## Resultat
  - Optimerade zoner för ballongplacering i 3D-volymen.
  - Tydlig påverkan av höjd på synlighet.
  - Riktningseffekter visualiserade via vektorfält.

  ![Vy 1](2026-04-29_15-45-32.png)
  ![Vy 2](2026-04-29_15-46-00.png)
  ![Vy 3](2026-04-29_15-46-08.png)
  ![Vy 4](2026-04-29_15-46-23.png)
