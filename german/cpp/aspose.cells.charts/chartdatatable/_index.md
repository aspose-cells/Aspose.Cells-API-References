---
title: Aspose::Cells::Charts::ChartDataTable class
linktitle: ChartDataTable
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartDataTable class. Represents a chart data table in C++.'
type: docs
weight: 700
url: /de/cpp/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class


Represents a chart data table.

```cpp
class ChartDataTable
```

## Methods

| Method | Description |
| --- | --- |
| [ChartDataTable(ChartDataTable_Impl* impl)](./chartdatatable/) | Constructs from an implementation object. |
| [ChartDataTable(const ChartDataTable\& src)](./chartdatatable/) | Copy constructor. |
| [GetAutoScaleFont()](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [GetBackgroundMode()](./getbackgroundmode/) | Gets and sets the display mode of the background. |
| [GetBorder()](./getborder/) | Returns a [Border](../../aspose.cells/border/) object that represents the border of the object. |
| [GetFont()](./getfont/) | Gets a [Font](../../aspose.cells/font/) object which represents the font setting of the specified chart data table. |
| [GetHasBorderHorizontal()](./gethasborderhorizontal/) |  **(Deprecated)** True if the chart data table has horizontal cell borders. |
| [GetHasBorderOutline()](./gethasborderoutline/) |  **(Deprecated)** True if the chart data table has outline borders. |
| [GetHasBorderVertical()](./gethasbordervertical/) |  **(Deprecated)** True if the chart data table has vertical cell borders. |
| [GetHasHorizontalBorder()](./gethashorizontalborder/) | True if the chart data table has horizontal cell borders. |
| [GetHasOutlineBorder()](./gethasoutlineborder/) | True if the chart data table has outline borders. |
| [GetHasVerticalBorder()](./gethasverticalborder/) | True if the chart data table has vertical cell borders. |
| [GetShowLegendKey()](./getshowlegendkey/) | True if the data label legend key is visible. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartDataTable\& src)](./operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](./setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetHasBorderHorizontal(bool value)](./sethasborderhorizontal/) |  **(Deprecated)** True if the chart data table has horizontal cell borders. |
| [SetHasBorderOutline(bool value)](./sethasborderoutline/) |  **(Deprecated)** True if the chart data table has outline borders. |
| [SetHasBorderVertical(bool value)](./sethasbordervertical/) |  **(Deprecated)** True if the chart data table has vertical cell borders. |
| [SetHasHorizontalBorder(bool value)](./sethashorizontalborder/) | True if the chart data table has horizontal cell borders. |
| [SetHasOutlineBorder(bool value)](./sethasoutlineborder/) | True if the chart data table has outline borders. |
| [SetHasVerticalBorder(bool value)](./sethasverticalborder/) | True if the chart data table has vertical cell borders. |
| [SetShowLegendKey(bool value)](./setshowlegendkey/) | True if the data label legend key is visible. |
| [~ChartDataTable()](./~chartdatatable/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
    //Instanziieren eines Workbook-Objekts
    Workbook workbook;

    //Abrufen der Referenz des ersten Arbeitsblatts
    Worksheet worksheet = workbook.GetWorksheets().Get(0);

    //Füge einen Beispielwert zur Zelle "A1" hinzu
    worksheet.GetCells().Get(u"A1").PutValue(50);

    //Füge einen Beispielwert zur Zelle "A2" hinzu
    worksheet.GetCells().Get(u"A2").PutValue(100);

    //Füge einen Beispielwert zur Zelle "A3" hinzu
    worksheet.GetCells().Get(u"A3").PutValue(150);

    //Füge einen Beispielwert zur Zelle "B1" hinzu
    worksheet.GetCells().Get(u"B1").PutValue(60);

    //Füge einen Beispielwert zur Zelle "B2" hinzu
    worksheet.GetCells().Get(u"B2").PutValue(32);

    //Füge einen Beispielwert zur Zelle "B3" hinzu
    worksheet.GetCells().Get(u"B3").PutValue(50);

    //Hinzufügen eines Diagramms zum Arbeitsblatt
    int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 25, 10);

    //Zugriff auf die Instanz des neu hinzugefügten Diagramms
    Chart chart = worksheet.GetCharts().Get(chartIndex);

    //Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm, das von der Zelle "A1" bis "B3" reicht
    chart.GetNSeries().Add(u"A1:B3", true);

    chart.SetShowDataTable(true);

    //Abrufen der Diagrammtabelle
    ChartDataTable chartTable = chart.GetChartDataTable();

    //Festlegen der Schriftfarbe der Diagrammtabelle
    chartTable.GetFont().SetColor(Color{ 0xff, 0xff, 0, 0 });

    //Festlegen der Sichtbarkeitsoptionen für das Legenden‑Schlüssel
    chartTable.SetShowLegendKey(false);

    //Speichern der Excel-Datei
    workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
