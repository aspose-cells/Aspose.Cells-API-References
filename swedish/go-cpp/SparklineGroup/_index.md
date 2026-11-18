---
title: "SparklineGroup-klass"
linktitle: "SparklineGroup"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SparklineGroup-klass. Inkapslar objektet som representerar sparklinegroup i Go."
type: docs
weight: 200
url: /sv/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref="Sparkline"/> organiseras i en sparkline-grupp. En SparklineGroup innehåller ett variabelt antal sparkline‑element. En sparkline‑grupp specificerar typen, displayinställningarna och axelinställningarna för sparkline‑elementen.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | Återställer dataområdet och platsområdet för sparkline-gruppen. Denna metod rensar ursprungliga sparkline-objekt i gruppen och skapar nya sparkline-objekt för de nya områdena. |
| [GetPresetStyle](./getpresetstyle/) | Hämtar och anger den förinställda stiltypen för sparkline-gruppen. |
| [SetPresetStyle](./setpresetstyle/) | Hämtar och anger den förinställda stiltypen för sparkline-gruppen. |
| [GetSparklines](./getsparklines/) | Hämtar samlingen av Sparkline-objekt. |
| [GetType](./gettype/) | Anger sparkline-typen för sparkline-gruppen. |
| [SetType](./settype/) | Anger sparkline-typen för sparkline-gruppen. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Anger hur tomma celler ska plottas. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Anger hur tomma celler ska plottas. |
| [GetDisplayHidden](./getdisplayhidden/) | Anger om data ska visas i dolda rader och kolumner. |
| [SetDisplayHidden](./setdisplayhidden/) | Anger om data ska visas i dolda rader och kolumner. |
| [GetShowHighPoint](./getshowhighpoint/) | Anger om de högsta datapunkterna i sparkline-gruppen ska markeras. |
| [SetShowHighPoint](./setshowhighpoint/) | Anger om de högsta datapunkterna i sparkline-gruppen ska markeras. |
| [GetHighPointColor](./gethighpointcolor/) | Hämtar och anger färgen på de högsta datapunkterna i sparkline-gruppen. |
| [SetHighPointColor](./sethighpointcolor/) | Hämtar och anger färgen på de högsta datapunkterna i sparkline-gruppen. |
| [GetShowLowPoint](./getshowlowpoint/) | Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras. |
| [SetShowLowPoint](./setshowlowpoint/) | Anger om de lägsta datapunkterna i sparkline-gruppen ska markeras. |
| [GetLowPointColor](./getlowpointcolor/) | Hämtar och anger färgen på de lägsta datapunkterna i sparkline-gruppen. |
| [SetLowPointColor](./setlowpointcolor/) | Hämtar och anger färgen på de lägsta datapunkterna i sparkline-gruppen. |
| [GetShowNegativePoints](./getshownegativepoints/) | Anger om negativa värden i sparkline-gruppen ska markeras med en annan färg eller markör. |
| [SetShowNegativePoints](./setshownegativepoints/) | Anger om negativa värden i sparkline-gruppen ska markeras med en annan färg eller markör. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Hämtar och anger färgen på de negativa värdena i sparkline-gruppen. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Hämtar och anger färgen på de negativa värdena i sparkline-gruppen. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Anger om den första datapunkten i sparkline-gruppen ska markeras. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Anger om den första datapunkten i sparkline-gruppen ska markeras. |
| [GetFirstPointColor](./getfirstpointcolor/) | Hämtar och anger färgen på den första datapunkten i sparkline-gruppen. |
| [SetFirstPointColor](./setfirstpointcolor/) | Hämtar och anger färgen på den första datapunkten i sparkline-gruppen. |
| [GetShowLastPoint](./getshowlastpoint/) | Anger om den sista datapunkten i sparkline-gruppen ska markeras. |
| [SetShowLastPoint](./setshowlastpoint/) | Anger om den sista datapunkten i sparkline-gruppen ska markeras. |
| [GetLastPointColor](./getlastpointcolor/) | Hämtar och anger färgen på den sista datapunkten i sparkline-gruppen. |
| [SetLastPointColor](./setlastpointcolor/) | Hämtar och anger färgen på den sista datapunkten i sparkline-gruppen. |
| [GetShowMarkers](./getshowmarkers/) | Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras. |
| [SetShowMarkers](./setshowmarkers/) | Anger om varje punkt i varje linjesparkline i sparkline-gruppen ska markeras. |
| [GetMarkersColor](./getmarkerscolor/) | Hämtar och anger färgen på punkterna i varje linjesparkline i sparkline-gruppen. |
| [SetMarkersColor](./setmarkerscolor/) | Hämtar och anger färgen på punkterna i varje linjesparkline i sparkline-gruppen. |
| [GetSeriesColor](./getseriescolor/) | Hämtar och anger färgen på sparkline-diagrammen i sparkline-gruppen. |
| [SetSeriesColor](./setseriescolor/) | Hämtar och anger färgen på sparkline-diagrammen i sparkline-gruppen. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Anger om plottdatan är från höger till vänster. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Anger om plottdatan är från höger till vänster. |
| [GetLineWeight](./getlineweight/) | Hämtar och anger linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter. |
| [SetLineWeight](./setlineweight/) | Hämtar och anger linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Hämtar och anger färgen på den horisontella axeln i sparkline-gruppen. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Hämtar och anger färgen på den horisontella axeln i sparkline-gruppen. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Anger om den horisontella axeln för sparkline ska visas. Den horisontella axeln visas om sparkline har data som korsar nollaxeln. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Representerar intervallet som innehåller datumvärdena för sparkline-data. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Representerar intervallet som innehåller datumvärdena för sparkline-data. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Representerar den vertikala axelns maxvärdestyp. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Representerar den vertikala axelns maxvärdestyp. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Hämtar och anger det anpassade maxvärdet för den vertikala axeln. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Hämtar och anger det anpassade maxvärdet för den vertikala axeln. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Anger det anpassade maxvärdet för sparkline-axelns vertikala axel med den angivna axelvärdestypen. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Anger det anpassade minvärdet för sparkline-axelns vertikala axel med den angivna axelvärdestypen. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Representerar den vertikala axelns minvärdestyp. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Representerar den vertikala axelns minvärdestyp. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Hämtar och anger det anpassade minvärdet för den vertikala axeln. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Hämtar och anger det anpassade minvärdet för den vertikala axeln. |
