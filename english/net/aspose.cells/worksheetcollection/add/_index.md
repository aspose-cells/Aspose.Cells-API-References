---
title: WorksheetCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds a worksheet to the collection
type: docs
url: /net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Adds a worksheet to the collection.

```csharp
public int Add(SheetType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | SheetType | Worksheet type. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();
workbook.Worksheets.Add(SheetType.Chart);
Cells cells = workbook.Worksheets[0].Cells;
cells["c2"].PutValue(5000);
cells["c3"].PutValue(3000);
cells["c4"].PutValue(4000);
cells["c5"].PutValue(5000);
cells["c6"].PutValue(6000);
ChartCollection charts = workbook.Worksheets[1].Charts;
int chartIndex = charts.Add(ChartType.Column, 10,10,20,20);
Chart chart = charts[chartIndex];
chart.NSeries.Add("Sheet1!C2:C6", true);

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
workbook.Worksheets.Add(SheetType.Chart)
Dim cells As Cells = workbook.Worksheets(0).Cells 
cells("c2").PutValue(5000)
cells("c3").PutValue(3000)
cells("c4").PutValue(4000)
cells("c5").PutValue(5000)
cells("c6").PutValue(6000)
Dim charts As ChartCollection = workbook.Worksheets(1).Charts
Dim chartIndex As Integer = charts.Add(ChartType.Column,10,10,20,20) 
Dim chart As Chart = charts(chartIndex) 
chart.NSeries.Add("Sheet1!C2:C6", True)
```

### See Also

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Adds a worksheet to the collection.

```csharp
public int Add()
```

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Examples

```csharp
// Called: Worksheet addedSheet = newWorkbook.Worksheets[newWorkbook.Worksheets.Add()];
[Test]
        public void Method_Add()
        {
            Workbook sourceWorkbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet537011.xlsm");
            Workbook newWorkbook = new Aspose.Cells.Workbook();
            foreach (Worksheet sourceWorksheet in sourceWorkbook.Worksheets)
            {
                // Copy the worksheets to newWorkbook
                //var sourceWorksheet = sourceWorkbook.Worksheets[worksheet];
                Worksheet addedSheet = newWorkbook.Worksheets[newWorkbook.Worksheets.Add()];
                // addedSheet.MoveTo(0);
                addedSheet.Copy(sourceWorksheet);
            }

            //// Clone the newWorkbook and Save 
            Workbook result = new Workbook();
            result.Copy(newWorkbook);
            //}
            sourceWorkbook.Save(Constants.destPath + "CellsNet537011_1.xlsx");
            newWorkbook.Save(Constants.destPath + "CellsNet537011_2.xlsx");
            result.Save(Constants.destPath + "CellsNet537011_3.xlsx");
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Adds a worksheet to the collection.

```csharp
public Worksheet Add(string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |

### Return Value

[`Worksheet`](../../worksheet/) object.

### Examples

```csharp
// Called: Worksheet newSheet = destinationWorkbook.Worksheets.Add(sourceSheet.Name);
[Test]
        public void Method_String_()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath + "CELLSNET57311.xlsx");
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Worksheets.RemoveAt(0);
            for (int i = 0; i < sourceWorkbook.Worksheets.Count; i++)
            {
                Worksheet sourceSheet = sourceWorkbook.Worksheets[i];
                Worksheet newSheet = destinationWorkbook.Worksheets.Add(sourceSheet.Name);
                newSheet.Copy(sourceSheet);
            }
           Assert.AreEqual("=test",destinationWorkbook.Worksheets[0].ConditionalFormattings[0][0].Formula1);
            destinationWorkbook.Save(Constants.destPath +"CELLSNET57311.xlsx");

        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


