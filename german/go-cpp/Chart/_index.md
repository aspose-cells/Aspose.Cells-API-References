---
title: "Chart Klasse"
linktitle: "Chart"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Chart-Klasse. Kapselt das Objekt, das ein Diagramm in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/chart/
---

## Chart class

Kapselt das Objekt, das ein einzelnes Excel‑Diagramm darstellt.

```go

type Chart struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetStyle](./getstyle/) | Liest und setzt den integrierten Stil. |
| [SetStyle](./setstyle/) | Liest und setzt den integrierten Stil. |
| [GetChartObject](./getchartobject/) | Stellt das chartShape dar; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Gibt an, ob die Pivot-Diagramm-Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Gibt an, ob die Pivot-Diagramm-Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist. |
| [GetPivotOptions](./getpivotoptions/) | Gibt die Pivot-Steuerelemente an, die im Diagramm angezeigt werden |
| [GetPivotSource](./getpivotsource/) | Die Quelle sind die Daten der Pivot-Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart. |
| [SetPivotSource](./setpivotsource/) | Die Quelle sind die Daten der Pivot-Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Gibt zurück, ob die vom Diagramm referenzierte Zelle vorhanden ist. |
| [IsChartDataChanged](./ischartdatachanged/) | Erkennt, ob die Datenquelle eines Diagramms geändert wurde. |
| [GetPlotBy](./getplotby/) | Liest und setzt, ob nach Zeile oder Spalte geplottet wird. |
| [RefreshPivotData](./refreshpivotdata/) | Aktualisiert die Diagrammdaten aus der Pivot-Tabelle. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Liest und setzt, wie leere Zellen geplottet werden. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Liest und setzt, wie leere Zellen geplottet werden. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | Gibt an, ob #N/A als leerer Wert angezeigt werden soll. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | Gibt an, ob #N/A als leerer Wert angezeigt werden soll. |
| [GetName](./getname/) | Liest und setzt den Namen des Diagramms. |
| [SetName](./setname/) | Liest und setzt den Namen des Diagramms. |
| [GetSizeWithWindow](./getsizewithwindow/) | Wahr, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst. |
| [SetSizeWithWindow](./setsizewithwindow/) | Wahr, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst. |
| [GetWorksheet](./getworksheet/) | Liest das Arbeitsblatt, das dieses Diagramm enthält. |
| [GetShapes](./getshapes/) | Gibt alle Zeichenformen in diesem Diagramm zurück. |
| [GetPrintSize](./getprintsize/) | Liest und setzt die gedruckte Diagrammgröße. |
| [SetPrintSize](./setprintsize/) | Liest und setzt die gedruckte Diagrammgröße. |
| [ChangeTemplate](./changetemplate/) | Diagrammtyp mit einer vordefinierten Vorlage ändern. |
| [GetType](./gettype/) | Liest oder setzt den Typ eines Diagramms. |
| [SetType](./settype/) | Liest oder setzt den Typ eines Diagramms. |
| [Move](./move/) | Verschiebt das Diagramm an einen angegebenen Ort. |
| [GetNSeries](./getnseries/) | Liest eine SeriesCollection, die die Datenreihen im Diagramm darstellt. |
| [GetFilteredNSeries](./getfilterednseries/) | Liest eine SeriesCollection, die die im Diagramm gefilterten Datenreihen darstellt. |
| [GetTitle](./gettitle/) | Liest den Titel des Diagramms. |
| [GetSubTitle](./getsubtitle/) | Liest den Untertitel des Diagramms. Gilt nur für ODS-Dateien. |
| [GetPlotArea](./getplotarea/) | Ruft den Plotbereich des Diagramms ab, der Achsentick‑Beschriftungen enthält. |
| [GetChartArea](./getchartarea/) | Ruft den Diagrammbereich im Arbeitsblatt ab. |
| [GetCategoryAxis](./getcategoryaxis/) | Ruft die X‑Achse des Diagramms ab. |
| [GetValueAxis](./getvalueaxis/) | Ruft die Y‑Achse des Diagramms ab. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Ruft die zweite Y‑Achse des Diagramms ab. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Ruft die zweite X‑Achse des Diagramms ab. |
| [GetSeriesAxis](./getseriesaxis/) | Ruft die Reihen‑Achse des Diagramms ab. |
| [GetLegend](./getlegend/) | Ruft die Diagrammlegende ab. |
| [GetChartDataTable](./getchartdatatable/) | Stellt die Diagrammdatentabelle dar. |
| [GetShowLegend](./getshowlegend/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true. |
| [SetShowLegend](./setshowlegend/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true. |
| [IsRectangularCornered](./isrectangularcornered/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob der Diagrammbereich rechteckig mit Ecken ist. Standard ist true. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob der Diagrammbereich rechteckig mit Ecken ist. Standard ist true. |
| [GetShowDataTable](./getshowdatatable/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [SetShowDataTable](./setshowdatatable/) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Ruft den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments ab oder legt ihn fest, in Grad (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen‑, 3‑D‑Kuchen‑ und Donut‑Diagramme, 0 bis 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Ruft den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments ab oder legt ihn fest, in Grad (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen‑, 3‑D‑Kuchen‑ und Donut‑Diagramme, 0 bis 360. |
| [GetGapWidth](./getgapwidth/) | Ruft den Abstand zwischen Balken‑ oder Säulen‑Clustern ab oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [SetGapWidth](./setgapwidth/) | Ruft den Abstand zwischen Balken‑ oder Säulen‑Clustern ab oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [GetGapDepth](./getgapdepth/) | Ruft den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm ab oder legt ihn fest, als Prozentsatz der Markierungsbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [SetGapDepth](./setgapdepth/) | Ruft den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm ab oder legt ihn fest, als Prozentsatz der Markierungsbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [Calculate](./calculate/) | Berechnet die benutzerdefinierten Positionen des Plotbereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Berechnet die benutzerdefinierte Position des Plotbereichs und der Achsen, wenn deren Position automatisch zugewiesen wird, mit Diagramm‑Berechnungsoptionen. |
| [GetFloor](./getfloor/) | Gibt ein Floor‑Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt. |
| [GetWalls](./getwalls/) | Gibt ein Walls‑Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt. |
| [GetBackWall](./getbackwall/) | Gibt ein Walls‑Objekt zurück, das die Rückwand eines 3‑D‑Diagramms darstellt. |
| [GetSideWall](./getsidewall/) | Gibt ein Walls‑Objekt zurück, das die Seitenwand eines 3‑D‑Diagramms darstellt. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | True, wenn Gitternetzlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | True, wenn Gitternetzlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden. |
| [GetRotationAngle](./getrotationangle/) | Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Plotbereichs um die Z‑Achse, in Grad). |
| [SetRotationAngle](./setrotationangle/) | Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Plotbereichs um die Z‑Achse, in Grad). |
| [GetElevation](./getelevation/) | Stellt die Höhe der 3‑D‑Diagrammansicht dar, in Grad. |
| [SetElevation](./setelevation/) | Stellt die Höhe der 3‑D‑Diagrammansicht dar, in Grad. |
| [GetRightAngleAxes](./getrightangleaxes/) | True, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3‑D‑Diagramme (außer Column3D und 3‑D‑Kuchen‑Diagrammen). |
| [SetRightAngleAxes](./setrightangleaxes/) | True, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3‑D‑Diagramme (außer Column3D und 3‑D‑Kuchen‑Diagrammen). |
| [GetAutoScaling](./getautoscaling/) | Wahr, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es der Größe des entsprechenden 2‑D‑Diagramms näher kommt. Die Eigenschaft RightAngleAxes muss True sein. |
| [SetAutoScaling](./setautoscaling/) | Wahr, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es der Größe des entsprechenden 2‑D‑Diagramms näher kommt. Die Eigenschaft RightAngleAxes muss True sein. |
| [GetHeightPercent](./getheightpercent/) | Gibt die Höhe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite zurück oder legt sie fest (zwischen 5 % und 500 %). |
| [SetHeightPercent](./setheightpercent/) | Gibt die Höhe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite zurück oder legt sie fest (zwischen 5 % und 500 %). |
| [GetPerspective](./getperspective/) | Gibt die Perspektive für die dreidimensionale Diagrammansicht zurück oder legt sie fest. Muss zwischen 0 und 100 liegen. Diese Eigenschaft wird ignoriert, wenn die Eigenschaft RightAngleAxes True ist. |
| [SetPerspective](./setperspective/) | Gibt die Perspektive für die dreidimensionale Diagrammansicht zurück oder legt sie fest. Muss zwischen 0 und 100 liegen. Diese Eigenschaft wird ignoriert, wenn die Eigenschaft RightAngleAxes True ist. |
| [GetIs3D](./getis3d/) | Gibt an, ob das Diagramm ein 3‑D‑Diagramm ist. |
| [GetDepthPercent](./getdepthpercent/) | Stellt die Tiefe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 % und 2000 %). |
| [SetDepthPercent](./setdepthpercent/) | Stellt die Tiefe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 % und 2000 %). |
| [ToImage_String](./toimage_string/) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp. |
| [ToImage_Int64](./toimage_int64/) | Erstellt das Diagrammbild und speichert es in einem Stream im JPEG‑Format. |
| [ToImage_ImageType](./toimage_imagetype/) | Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format. |
| [ToPdf_String](./topdf_string/) | Speichert das Diagramm in einer PDF‑Datei. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Speichert das Diagramm in einer PDF‑Datei. |
| [ToPdf](./topdf/) | Erstellt das Diagramm‑PDF und speichert es in einem Stream. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Erstellt das Diagramm‑PDF und speichert es in einem Stream. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format. |
| [GetActualSize](./getactualsize/) | Ermittelt die tatsächliche Größe des Diagramms in Pixeln. |
| [GetPlacement](./getplacement/) | Stellt dar, wie das Diagramm an den darunterliegenden Zellen befestigt ist. |
| [SetPlacement](./setplacement/) | Stellt dar, wie das Diagramm an den darunterliegenden Zellen befestigt ist. |
| [GetPageSetup](./getpagesetup/) | Stellt die Seitenlayout‑Beschreibung dieses Diagramms dar. |
| [HasAxis](./hasaxis/) | Gibt zurück, welche Achsen im Diagramm vorhanden sind. |
| [SwitchRowColumn](./switchrowcolumn/) | Vertauscht Zeile/Spalte. |
| [GetChartDataRange](./getchartdatarange/) | Ermittelt den Datenquellenbereich des Diagramms. |
| [SetChartDataRange](./setchartdatarange/) | Gibt den Datenbereich für ein Diagramm an. |
| [GetLine](./getline/) | Ermittelt die Linie. |
