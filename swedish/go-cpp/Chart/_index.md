---
title: "Chart klass"
linktitle: "Chart"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Chart-klass. Inkapslar objektet som representerar chart i Go."
type: docs
weight: 200
url: /sv/go-cpp/chart/
---

## Chart class

Inkapslar objektet som representerar ett enskilt Excel-diagram.

```go

type Chart struct  {
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
| [GetStyle](./getstyle/) | Hämtar och anger den inbyggda stilen. |
| [SetStyle](./setstyle/) | Hämtar och anger den inbyggda stilen. |
| [GetChartObject](./getchartobject/) | Representerar chartShape; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Anger om fältknapparna för pivottabellens diagram ska döljas endast när diagrammet är ett PivotChart. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Anger om fältknapparna för pivottabellens diagram ska döljas endast när diagrammet är ett PivotChart. |
| [GetPivotOptions](./getpivotoptions/) | Specificerar pivotkontrollerna som visas på diagrammet. |
| [GetPivotSource](./getpivotsource/) | Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart. |
| [SetPivotSource](./setpivotsource/) | Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Returnerar om cellen som diagrammet refererar till. |
| [IsChartDataChanged](./ischartdatachanged/) | Detekterar om ett diagrams datakälla har ändrats. |
| [GetPlotBy](./getplotby/) | Hämtar och anger om diagrammet ska plottas radvis eller kolumnvis. |
| [RefreshPivotData](./refreshpivotdata/) | Uppdaterar diagrammets data från pivottabell. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Hämtar och anger hur tomma celler ska plottas. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Hämtar och anger hur tomma celler ska plottas. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Anger om endast synliga celler ska plottas. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Anger om endast synliga celler ska plottas. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | Anger om #N/A ska visas som ett tomt värde. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | Anger om #N/A ska visas som ett tomt värde. |
| [GetName](./getname/) | Hämtar och anger diagrammets namn. |
| [SetName](./setname/) | Hämtar och anger diagrammets namn. |
| [GetSizeWithWindow](./getsizewithwindow/) | Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster. |
| [SetSizeWithWindow](./setsizewithwindow/) | Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster. |
| [GetWorksheet](./getworksheet/) | Hämtar arbetsbladet som innehåller detta diagram. |
| [GetShapes](./getshapes/) | Returnerar alla ritningsformer i detta diagram. |
| [GetPrintSize](./getprintsize/) | Hämtar och anger den utskrivna diagramstorleken. |
| [SetPrintSize](./setprintsize/) | Hämtar och anger den utskrivna diagramstorleken. |
| [ChangeTemplate](./changetemplate/) | Ändra diagramtyp med en förinställd mall. |
| [GetType](./gettype/) | Hämtar eller anger ett diagrams typ. |
| [SetType](./settype/) | Hämtar eller anger ett diagrams typ. |
| [Move](./move/) | Flyttar diagrammet till en angiven plats. |
| [GetNSeries](./getnseries/) | Hämtar en SeriesCollection-samling som representerar dataserierna i diagrammet. |
| [GetFilteredNSeries](./getfilterednseries/) | Hämtar en SeriesCollection-samling som representerar dataserierna som är filtrerade i diagrammet. |
| [GetTitle](./gettitle/) | Hämtar diagrammets titel. |
| [GetSubTitle](./getsubtitle/) | Hämtar diagrammets undertitel. Gäller endast ODS-filer. |
| [GetPlotArea](./getplotarea/) | Hämtar diagrammets plotområde som inkluderar axelns tick-etiketter. |
| [GetChartArea](./getchartarea/) | Hämtar diagramområdet i arbetsbladet. |
| [GetCategoryAxis](./getcategoryaxis/) | Hämtar diagrammets X-axel. |
| [GetValueAxis](./getvalueaxis/) | Hämtar diagrammets Y-axel. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Hämtar diagrammets andra Y-axel. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Hämtar diagrammets andra X-axel. |
| [GetSeriesAxis](./getseriesaxis/) | Hämtar diagrammets serieraxel. |
| [GetLegend](./getlegend/) | Hämtar diagrammets förklaring. |
| [GetChartDataTable](./getchartdatatable/) | Representerar diagrammets datatabell. |
| [GetShowLegend](./getshowlegend/) | Hämtar eller anger ett värde som indikerar om diagrammets förklaring ska visas. Standard är true. |
| [SetShowLegend](./setshowlegend/) | Hämtar eller anger ett värde som indikerar om diagrammets förklaring ska visas. Standard är true. |
| [IsRectangularCornered](./isrectangularcornered/) | Hämtar eller anger ett värde som indikerar om diagramområdet har rektangulära hörn. Standard är true. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Hämtar eller anger ett värde som indikerar om diagramområdet har rektangulära hörn. Standard är true. |
| [GetShowDataTable](./getshowdatatable/) | Hämtar eller anger ett värde som indikerar om diagrammet visar en datatabell. |
| [SetShowDataTable](./setshowdatatable/) | Hämtar eller anger ett värde som indikerar om diagrammet visar en datatabell. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Hämtar eller anger vinkeln för den första paj- eller munkdiagramsegmentet, i grader (medurs från vertikal).Gäller endast för paj, 3-D-paj och munkdiagram, 0 till 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Hämtar eller anger vinkeln för den första paj- eller munkdiagramsegmentet, i grader (medurs från vertikal).Gäller endast för paj, 3-D-paj och munkdiagram, 0 till 360. |
| [GetGapWidth](./getgapwidth/) | Returnerar eller anger avståndet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [SetGapWidth](./setgapwidth/) | Returnerar eller anger avståndet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [GetGapDepth](./getgapdepth/) | Hämtar eller anger avståndet mellan dataserier i ett 3-D-diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [SetGapDepth](./setgapdepth/) | Hämtar eller anger avståndet mellan dataserier i ett 3-D-diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste vara mellan 0 och 500. |
| [Calculate](./calculate/) | Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner tilldelas automatiskt. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Beräknar den anpassade positionen för plotområdet och axlarna om deras positioner tilldelas automatiskt, med Diagramberäkningsalternativ. |
| [GetFloor](./getfloor/) | Returnerar ett Floor-objekt som representerar väggarna i ett 3-D-diagram. |
| [GetWalls](./getwalls/) | Returnerar ett Walls-objekt som representerar väggarna i ett 3-D-diagram. |
| [GetBackWall](./getbackwall/) | Returnerar ett Walls-objekt som representerar bakväggen i ett 3-D-diagram. |
| [GetSideWall](./getsidewall/) | Returnerar ett Walls-objekt som representerar sidoväggen i ett 3-D-diagram. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram. |
| [GetRotationAngle](./getrotationangle/) | Representerar rotationen av 3-D-diagrambilden (rotationen av plotområdet runt z-axeln, i grader). |
| [SetRotationAngle](./setrotationangle/) | Representerar rotationen av 3-D-diagrambilden (rotationen av plotområdet runt z-axeln, i grader). |
| [GetElevation](./getelevation/) | Representerar höjden på 3-D-diagrambilden, i grader. |
| [SetElevation](./setelevation/) | Representerar höjden på 3-D-diagrambilden, i grader. |
| [GetRightAngleAxes](./getrightangleaxes/) | Sant om diagramaxlarna är i räta vinklar. Gäller endast för 3-D-diagram (förutom Column3D och 3-D-pajdiagram). |
| [SetRightAngleAxes](./setrightangleaxes/) | Sant om diagramaxlarna är i räta vinklar. Gäller endast för 3-D-diagram (förutom Column3D och 3-D-pajdiagram). |
| [GetAutoScaling](./getautoscaling/) | Sant om Microsoft Excel skalar ett 3-D-diagram så att det är närmare i storlek till motsvarande 2-D-diagram. RightAngleAxes-egenskapen måste vara True. |
| [SetAutoScaling](./setautoscaling/) | Sant om Microsoft Excel skalar ett 3-D-diagram så att det är närmare i storlek till motsvarande 2-D-diagram. RightAngleAxes-egenskapen måste vara True. |
| [GetHeightPercent](./getheightpercent/) | Returnerar eller anger höjden på ett 3-D-diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [SetHeightPercent](./setheightpercent/) | Returnerar eller anger höjden på ett 3-D-diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [GetPerspective](./getperspective/) | Returnerar eller anger perspektivet för den tredimensionella diagrambilden. Måste vara mellan 0 och 100. Denna egenskap ignoreras om RightAngleAxes-egenskapen är True. |
| [SetPerspective](./setperspective/) | Returnerar eller anger perspektivet för den tredimensionella diagrambilden. Måste vara mellan 0 och 100. Denna egenskap ignoreras om RightAngleAxes-egenskapen är True. |
| [GetIs3D](./getis3d/) | Indikerar om diagrammet är ett 3D-diagram. |
| [GetDepthPercent](./getdepthpercent/) | Representerar djupet på ett 3-D-diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [SetDepthPercent](./setdepthpercent/) | Representerar djupet på ett 3-D-diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [ToImage_String](./toimage_string/) | Skapar diagrambilden och sparar den till en fil. Filändelsen bestämmer bildformatet. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Skapar diagrambilden och sparar den till en fil i den angivna bildtypen. |
| [ToImage_Int64](./toimage_int64/) | Skapar diagrambilden och sparar den till en ström i JPEG-format. |
| [ToImage_ImageType](./toimage_imagetype/) | Skapar diagrambilden och sparar den till en ström i det angivna formatet. |
| [ToPdf_String](./topdf_string/) | Sparar diagrammet till en PDF-fil. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Sparar diagrammet till en PDF-fil. |
| [ToPdf](./topdf/) | Skapar diagram-PDF och sparar den till en ström. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Skapar diagram-pdf och sparar den till en ström. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Skapar diagrambilden och sparar den till en fil. Filändelsen bestämmer bildformatet. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Skapar diagrambilden och sparar den till en ström i det angivna formatet. |
| [GetActualSize](./getactualsize/) | Hämtar den faktiska storleken på diagrammet i enheten pixlar. |
| [GetPlacement](./getplacement/) | Representerar hur diagrammet är fäst vid cellerna under det. |
| [SetPlacement](./setplacement/) | Representerar hur diagrammet är fäst vid cellerna under det. |
| [GetPageSetup](./getpagesetup/) | Representerar sidinställningsbeskrivningen i detta diagram. |
| [HasAxis](./hasaxis/) | Returnerar vilka axlar som finns på diagrammet. |
| [SwitchRowColumn](./switchrowcolumn/) | Växlar rad/kolumn. |
| [GetChartDataRange](./getchartdatarange/) | Hämtar datakällintervall för diagrammet. |
| [SetChartDataRange](./setchartdatarange/) | Anger dataintervall för ett diagram. |
| [GetLine](./getline/) | Hämtar linjen. |
