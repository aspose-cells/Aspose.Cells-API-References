---
title: "Serieklass"
linktitle: "Serie"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Serieklass. Inkapslar objektet som representerar serier i Go."
type: docs
weight: 200
url: /sv/go-cpp/series/
---

## Series class

Inkapslar objektet som representerar en enskild dataserie i ett diagram.

```go

type Series struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsFiltered](./isfiltered/) | Indikerar om serien är markerad eller filtrerad.True indikerar att denna serie är filtrerad, och den kommer inte att visas i diagrammet. |
| [SetIsFiltered](./setisfiltered/) | Indikerar om serien är markerad eller filtrerad.True indikerar att denna serie är filtrerad, och den kommer inte att visas i diagrammet. |
| [GetLayoutProperties](./getlayoutproperties/) | Representerar egenskaperna för layouten. |
| [Move](./move/) | Flyttar serien upp eller ner. |
| [GetPoints](./getpoints/) | Hämtar samlingen av punkter i en serie i ett diagram. |
| [GetArea](./getarea/) | Representerar bakgrundsområdet för Serie-objektet. |
| [GetBorder](./getborder/) | Representerar kanten på ett Serie-objekt. |
| [GetName](./getname/) | Hämtar eller anger namnet på dataserien. |
| [SetName](./setname/) | Hämtar eller anger namnet på dataserien. |
| [GetDisplayName](./getdisplayname/) | Hämtar seriens namn som visas i diagramgrafen. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Hämtar antalet datavärden. |
| [IsVerticalValues](./isverticalvalues/) | Indikerar om datakällan är vertikal. |
| [GetValues](./getvalues/) | Representerar Y-värdena för denna diagramserie. |
| [SetValues](./setvalues/) | Representerar Y-värdena för denna diagramserie. |
| [GetPointValues](./getpointvalues/) | Hämtar de faktiska värdena som används för att plotta varje pointof i denna serie i diagrammet. |
| [GetCategoryValues](./getcategoryvalues/) | Hämtar de faktiska kategorivärdena som används för att plotta varje pointof i denna serie i diagrammet. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Representerar formatkoden för Values NumberList. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Representerar formatkoden för Values NumberList. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | Representerar formatkoden för X Values' NumberList. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | Representerar formatkoden för X Values' NumberList. |
| [GetXValues](./getxvalues/) | Representerar X-värdena för denna diagramserie. |
| [SetXValues](./setxvalues/) | Representerar X-värdena för denna diagramserie. |
| [GetBubbleSizes](./getbubblesizes/) | Hämtar eller anger bubbelstorleksvärdena för diagramserien. |
| [SetBubbleSizes](./setbubblesizes/) | Hämtar eller anger bubbelstorleksvärdena för diagramserien. |
| [GetTrendLines](./gettrendlines/) | Returnerar alla trendlinjer för denna serie. |
| [GetSmooth](./getsmooth/) | Representerar kurvutjämning.True om kurvutjämning är påslagen för linjediagrammet eller spridningsdiagrammet.Gäller endast för linjediagram och spridningsdiagram med linjer. |
| [SetSmooth](./setsmooth/) | Representerar kurvutjämning.True om kurvutjämning är påslagen för linjediagrammet eller spridningsdiagrammet.Gäller endast för linjediagram och spridningsdiagram med linjer. |
| [GetShadow](./getshadow/) | True om serien har en skugga. |
| [SetShadow](./setshadow/) | True om serien har en skugga. |
| [GetHas3DEffect](./gethas3deffect/) | Sant om serien har ett tredimensionellt utseende. |
| [SetHas3DEffect](./sethas3deffect/) | Sant om serien har ett tredimensionellt utseende. |
| [GetBar3DShapeType](./getbar3dshapetype/) | Hämtar eller anger 3D-formtypen som används med 3-D stapel- eller kolumndiagram. |
| [SetBar3DShapeType](./setbar3dshapetype/) | Hämtar eller anger 3D-formtypen som används med 3-D stapel- eller kolumndiagram. |
| [GetDataLabels](./getdatalabels/) | Representerar DataLabels-objektet för den angivna ASeries. |
| [GetType](./gettype/) | Hämtar eller anger en dataserietyp. |
| [SetType](./settype/) | Hämtar eller anger en dataserietyp. |
| [GetMarker](./getmarker/) | Hämtar Marker</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Indikerar om denna serie plottas på den andra värdeaxeln. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Indikerar om denna serie plottas på den andra värdeaxeln. |
| [GetXErrorBar](./getxerrorbar/) | Representerar X-riktningens felstapeln för serien. |
| [GetYErrorBar](./getyerrorbar/) | Representerar Y-riktningens felstapeln för serien. |
| [GetHasHiLoLines](./gethashilolines/) | Sant om linjediagrammet har hög-låg-linjer.Gäller endast linjediagram. |
| [SetHasHiLoLines](./sethashilolines/) | Sant om linjediagrammet har hög-låg-linjer.Gäller endast linjediagram. |
| [GetHiLoLines](./gethilolines/) | Returnerar ett HiLoLines-objekt som representerar hög-låg-linjerna för en serie i ett linjediagram.Gäller endast linjediagram. |
| [GetHasSeriesLines](./gethasserieslines/) | Sant om ett staplat kolumndiagram eller staplat stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna.Gäller endast staplade kolumndiagram, staplade stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram. |
| [SetHasSeriesLines](./sethasserieslines/) | Sant om ett staplat kolumndiagram eller staplat stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna.Gäller endast staplade kolumndiagram, staplade stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram. |
| [GetSeriesLines](./getserieslines/) | Returnerar ett SeriesLines-objekt som representerar serielinjerna för ett staplat stapeldiagram eller ett staplat kolumndiagram.Gäller endast staplade stapeldiagram och staplade kolumndiagram. |
| [GetHasDropLines](./gethasdroplines/) | Sant om diagrammet har droplinjer.Gäller endast linjediagram eller områdesdiagram. |
| [SetHasDropLines](./sethasdroplines/) | Sant om diagrammet har droplinjer.Gäller endast linjediagram eller områdesdiagram. |
| [GetDropLines](./getdroplines/) | Returnerar ett Line-objekt som representerar droplinjerna för en serie i linjediagrammet eller områdesdiagrammet.Gäller endast linjediagram eller områdesdiagram. |
| [GetHasUpDownBars](./gethasupdownbars/) | Sant om ett linjediagram har upp- och nedåtbalkar.Gäller endast linjediagram. |
| [SetHasUpDownBars](./sethasupdownbars/) | Sant om ett linjediagram har upp- och nedåtbalkar.Gäller endast linjediagram. |
| [GetUpBars](./getupbars/) | Returnerar ett DropBars-objekt som representerar uppbalkarna i ett linjediagram.Gäller endast linjediagram. |
| [GetDownBars](./getdownbars/) | Returnerar ett DropBars-objekt som representerar nedbalkarna i ett linjediagram.Gäller endast linjediagram. |
| [IsColorVaried](./iscolorvaried/) | Representerar om färgen på punkterna varierar.Diagrammet måste innehålla endast en serie eller så är detta diagram ett cirkeldiagram. |
| [SetIsColorVaried](./setiscolorvaried/) | Representerar om färgen på punkterna varierar.Diagrammet måste innehålla endast en serie eller så är detta diagram ett cirkeldiagram. |
| [GetGapWidth](./getgapwidth/) | Returnerar eller anger avståndet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [SetGapWidth](./setgapwidth/) | Returnerar eller anger avståndet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Hämtar eller anger vinkeln på den första paj- eller munkdiagramdelen, i grader (medurs från vertikal).Gäller endast paj-, 3-D paj- och munkdiagram, med värden från 0 till 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Hämtar eller anger vinkeln på den första paj- eller munkdiagramdelen, i grader (medurs från vertikal).Gäller endast paj-, 3-D paj- och munkdiagram, med värden från 0 till 360. |
| [GetOverlap](./getoverlap/) | Anger hur staplar och kolumner är placerade.Kan vara ett värde mellan -100 och 100.Gäller endast 2-D stapeldiagram och 2-D kolumndiagram. |
| [SetOverlap](./setoverlap/) | Anger hur staplar och kolumner är placerade.Kan vara ett värde mellan -100 och 100.Gäller endast 2-D stapeldiagram och 2-D kolumndiagram. |
| [GetSecondPlotSize](./getsecondplotsize/) | Returnerar eller anger storleken på den sekundära sektionen av antingen ett pie of pie-diagram eller ett bar of pie-diagram, som en procentandel av storleken på den primära pajen.Kan vara ett värde från 5 till 200. |
| [SetSecondPlotSize](./setsecondplotsize/) | Returnerar eller anger storleken på den sekundära sektionen av antingen ett pie of pie-diagram eller ett bar of pie-diagram, som en procentandel av storleken på den primära pajen.Kan vara ett värde från 5 till 200. |
| [GetSplitType](./getsplittype/) | Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett pie of pie- eller bar of pie-diagram. |
| [SetSplitType](./setsplittype/) | Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett pie of pie- eller bar of pie-diagram. |
| [GetSplitValue](./getsplitvalue/) | Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett pie of pie- eller bar of pie-diagram. |
| [SetSplitValue](./setsplitvalue/) | Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett pie of pie- eller bar of pie-diagram. |
| [IsAutoSplit](./isautosplit/) | Indikerar om tröskelvärdet är automatiskt. |
| [GetBubbleScale](./getbubblescale/) | Hämtar eller anger skalningsfaktorn för bubblor i den angivna diagramgruppen.Den kan vara ett heltal från 0 (noll) till 300, vilket motsvarar en procentandel av standardstorleken.Gäller endast bubbeldiagram. |
| [SetBubbleScale](./setbubblescale/) | Hämtar eller anger skalningsfaktorn för bubblor i den angivna diagramgruppen.Den kan vara ett heltal från 0 (noll) till 300, vilket motsvarar en procentandel av standardstorleken.Gäller endast bubbeldiagram. |
| [GetSizeRepresents](./getsizerepresents/) | Hämtar eller anger vad bubbelstorleken representerar i ett bubbeldiagram. |
| [SetSizeRepresents](./setsizerepresents/) | Hämtar eller anger vad bubbelstorleken representerar i ett bubbeldiagram. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | Sant om negativa bubblor visas för diagramgruppen. Giltigt endast för bubbeldiagram. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | Sant om negativa bubblor visas för diagramgruppen. Giltigt endast för bubbeldiagram. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentandel av diagrammets storlek, mellan 10 och 90 procent. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentandel av diagrammets storlek, mellan 10 och 90 procent. |
| [GetExplosion](./getexplosion/) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [SetExplosion](./setexplosion/) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | Sant om ett radardiagram har kategoriaxel-etiketter. Gäller endast för radardiagram. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | Sant om ett radardiagram har kategoriaxel-etiketter. Gäller endast för radardiagram. |
| [GetHasLeaderLines](./gethasleaderlines/) | Sant om serien har ledarlinjer. |
| [SetHasLeaderLines](./sethasleaderlines/) | Sant om serien har ledarlinjer. |
| [GetLeaderLines](./getleaderlines/) | Representerar ledarlinjer i ett diagram. Ledarlinjer kopplar datamärkningar till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enskild ledarlinje. |
| [GetLegendEntry](./getlegendentry/) | Hämtar förklaringsposten enligt denna serie. |
| [GetShapeProperties](./getshapeproperties/) | Hämtar ShapePropertyCollection-objektet som innehåller de visuella formegenskaperna för serien. |
