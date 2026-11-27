---
title: "Klass PivotFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFilter-klass. Representerar en PivotFilter i PivotFilter-samlingen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Representerar ett PivotFilter i PivotFilter-samlingen.

```csharp
public class PivotFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Föråldrad.**) Hämtar autofiltret för pivotfiltret. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Hämtar utvärderingsordningen för pivotfiltret. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Hämtar indexet för källfältet som detta pivotfilter tillämpas på. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Hämtar kategorin för detta filter. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Hämtar filtertypen för pivotfiltret. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Anger indexet för måttkubfältet. Denna egenskap används endast av filter i OLAP-pivoter och specificerar på vilket mått ett värdefilter ska tillämpas. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Föråldrad.**) Hämtar måttfältets index för pivotfiltret. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Hämtar medlemsegenskapsfältets index för pivotfiltret. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Hämtar namnet på pivotfiltret. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Anger om hela dagar ska användas i dess datumfiltreringskriterier. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Hämtar strängvärdet1 för etikettpivotfiltret. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Hämtar strängvärdet2 för etikettpivotfiltret. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Hämtar indexet för värdefältet i värdeområdet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Hämtar värden för talfiltret. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Hämtar etiketter för rubrikfiltret. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Hämtar värden för talfiltret. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Hämtar top‑10-inställningen för filtret. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i kalkylbladet med exempeldata
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

            // Lägg till en pivottabell i kalkylbladet
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Ställ in pivottabellens stil
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Lägg till ett pivotfilter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Ange ytterligare egenskaper för pivotfiltret
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Uppdatera och beräkna pivottabellens data
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


