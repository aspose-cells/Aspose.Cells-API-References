---
title: Class PivotFieldCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFieldCollection class. Represents a collection of all the PivotField objects in the different regions of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/
---
## PivotFieldCollection class

Represents a collection of all the PivotField objects in the different regions of the pivot table.

```csharp
public class PivotFieldCollection : CollectionBase<PivotField>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotfieldcollection/item/) { get; } | Gets the PivotField Object at the specific index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Type](../../aspose.cells.pivot/pivotfieldcollection/type/) { get; } | Gets the PivotFields type. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfieldcollection/add/)(PivotField) | Adds a PivotField Object to the specific type PivotFields. |
| [AddByBaseIndex](../../aspose.cells.pivot/pivotfieldcollection/addbybaseindex/)(int) | Adds a PivotField Object to the specific type PivotFields. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField, IComparer&lt;PivotField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotField, IComparer&lt;PivotField&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivotfieldcollection/clear/#clear)() | clear all fields of PivotFieldCollection (2 methods) |
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
| [Insert](../../aspose.cells.pivot/pivotfieldcollection/insert/)(int, PivotField) | Insert a pivot field at specific index. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int, int) |  |
| [Move](../../aspose.cells.pivot/pivotfieldcollection/move/)(int, int) | Moves the PivotField from current position to destination position |
| [Remove](../../aspose.cells.pivot/pivotfieldcollection/remove/)(PivotField) | Removes field from the current region. |
| [RemoveAt](../../aspose.cells.pivot/pivotfieldcollection/removeat/#removeat)(int) | Removes field by the index. Only for filter,row,column,data region. (2 methods) |

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
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

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Access the RowFields collection
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Display the count of row fields
            Console.WriteLine("Row Fields Count: " + rowFields.Count);

            // Access the first row field and display its name
            PivotField firstRowField = rowFields[0];
            Console.WriteLine("First Row Field Name: " + firstRowField.Name);

            // Add a new field by base index
            int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the "Year" field to the row area
            Console.WriteLine("New Field Index: " + newFieldIndex);

            // Clear all fields in the RowFields collection
            rowFields.Clear();
            Console.WriteLine("Row Fields Count after Clear: " + rowFields.Count);

            // Save the workbook
            workbook.Save("PivotFieldCollectionExample.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotField](../pivotfield/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


