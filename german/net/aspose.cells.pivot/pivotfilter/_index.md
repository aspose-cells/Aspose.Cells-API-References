---
title: "Klasse PivotFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotFilter class. Stellt einen PivotFilter in der PivotFilter‑Sammlung dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Stellt einen PivotFilter in der PivotFilter‑Sammlung dar.

```csharp
public class PivotFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Gibt den Autofilter des PivotFilters zurück. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Ermittelt die Auswertungsreihenfolge des Pivotfilters. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Ermittelt den Index des Quellfelds, auf das dieser Pivotfilter angewendet wird. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Ermittelt die Kategorie dieses Filters. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Ermittelt den Filtertyp des Pivotfilters. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Gibt den Index des Messwürfel-Feldes an. Diese Eigenschaft wird nur von Filtern in OLAP-Pivot-Tabellen verwendet und legt fest, auf welche Messgröße ein Wertfilter angewendet werden soll. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Ermittelt den Index des Messfelds des Pivotfilters. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Ermittelt den Index des Member-Property-Feldes des Pivotfilters. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Ermittelt den Namen des Pivotfilters. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Gibt an, ob bei den Datumsfilterkriterien ganze Tage verwendet werden sollen. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Ermittelt den Zeichenkettenwert1 des Beschriftungs-Pivotfilters. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Ermittelt den Zeichenkettenwert2 des Beschriftungs-Pivotfilters. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Ermittelt den Index des Wertefelds im Wertebereich. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Ermittelt die Werte des Zahlenfilters. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Ermittelt die Beschriftungen des Caption-Filters. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Ermittelt die Werte des Zahlenfilters. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Ermittelt die Top‑10‑Einstellung des Filters. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Arbeitsblatt mit Beispieldaten füllen
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // PivotTable-Stil festlegen
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Einen Pivotfilter hinzufügen
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Zusätzliche Eigenschaften für den Pivotfilter festlegen
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Aktualisieren und berechnen Sie die Pivot-Tabellendaten
            pivot.RefreshData();
            pivot.CalculateData();

            // Speichere die Arbeitsmappe
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


