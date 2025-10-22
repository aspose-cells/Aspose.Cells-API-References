##Class PivotFieldCollection
Aspose.Cells.Pivot.PivotFieldCollection class. Represents a collection of all the PivotField objects in the PivotTables specific PivotFields type
## PivotFieldCollection class
Represents a collection of all the PivotField objects in the PivotTable's specific PivotFields type.
```csharp
public class PivotFieldCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.pivot/pivotfieldcollection/count/) { get; } | Gets the count of the pivotFields. |
| [Item](../../aspose.cells.pivot/pivotfieldcollection/item/) { get; } | Gets the PivotField Object at the specific index. (2 indexers) |
| [Type](../../aspose.cells.pivot/pivotfieldcollection/type/) { get; } | Gets the PivotFields type. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfieldcollection/add/)(PivotField) | Adds a PivotField Object to the specific type PivotFields. |
| [AddByBaseIndex](../../aspose.cells.pivot/pivotfieldcollection/addbybaseindex/)(int) | Adds a PivotField Object to the specific type PivotFields. |
| [Clear](../../aspose.cells.pivot/pivotfieldcollection/clear/)() | clear all fields of PivotFieldCollection |
| [GetEnumerator](../../aspose.cells.pivot/pivotfieldcollection/getenumerator/)() | Gets an enumerator over the elements in this collection in proper sequence. |
| [Move](../../aspose.cells.pivot/pivotfieldcollection/move/)(int, int) | Moves the PivotField from current position to destination position |
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
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
