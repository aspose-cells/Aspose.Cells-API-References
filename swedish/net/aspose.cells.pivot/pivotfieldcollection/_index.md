---
title: "Klass PivotFieldCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldCollection-klass. Representerar en samling av alla PivotField-objekt i de olika regionerna i pivåttabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldcollection/
---
## PivotFieldCollection class

Representerar en samling av alla PivotField-objekt i de olika regionerna i pivottabellen.

```csharp
public class PivotFieldCollection : CollectionBase<PivotField>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotfieldcollection/item/) { get; } | Hämtar PivotField-objektet på det specifika indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Type](../../aspose.cells.pivot/pivotfieldcollection/type/) { get; } | Hämtar typen för PivotFields. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfieldcollection/add/)(PivotField) | Lägger till ett PivotField‑objekt till den specifika typen PivotFields. |
| [AddByBaseIndex](../../aspose.cells.pivot/pivotfieldcollection/addbybaseindex/)(int) | Lägger till ett PivotField‑objekt till den specifika typen PivotFields. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField, IComparer&lt;PivotField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotField, IComparer&lt;PivotField&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivotfieldcollection/clear/#clear)() | Rensa alla fält i PivotFieldCollection (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotField) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotField[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotField&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotField&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int, int) |  |
| [Insert](../../aspose.cells.pivot/pivotfieldcollection/insert/)(int, PivotField) | Infoga ett pivotfält på ett specifikt index. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int, int) |  |
| [Move](../../aspose.cells.pivot/pivotfieldcollection/move/)(int, int) | Flyttar PivotField från aktuell position till destinationspositionen |
| [Remove](../../aspose.cells.pivot/pivotfieldcollection/remove/)(PivotField) | Tar bort fält från den aktuella regionen. |
| [RemoveAt](../../aspose.cells.pivot/pivotfieldcollection/removeat/#removeat)(int) | Tar bort fält efter index. Endast för filter, rad, kolumn, dataregion. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionDemo
    {
        public static void PivotFieldCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Lägg till en pivottabell i kalkylbladet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Åtkomst till RowFields-samlingen
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Visa antalet radfält
            Console.WriteLine("Row Fields Count: " + rowFields.Count);

            // Åtkomst till det första radfältet och visa dess namn
            PivotField firstRowField = rowFields[0];
            Console.WriteLine("First Row Field Name: " + firstRowField.Name);

            // Lägg till ett nytt fält med basindex
            int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the "Year" field to the row area
            Console.WriteLine("New Field Index: " + newFieldIndex);

            // Rensa alla fält i RowFields-samlingen
            rowFields.Clear();
            Console.WriteLine("Row Fields Count after Clear: " + rowFields.Count);

            // Spara arbetsboken
            workbook.Save("PivotFieldCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotField](../pivotfield/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


