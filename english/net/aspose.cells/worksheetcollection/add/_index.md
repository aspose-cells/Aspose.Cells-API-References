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
// Called: workbook.Worksheets.Add();
public void WorksheetCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets.Add("!sheet 2");
    workbook.Worksheets.Add();
    string str = string.Format("'{0}'!A1", workbook.Worksheets[1].Name);
    workbook.Worksheets[2].Hyperlinks.Add(2, 1, 1, 1, str);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Hyperlink link = workbook.Worksheets[2].Hyperlinks[0];
    Assert.AreEqual(str, link.Address);
    Assert.AreEqual(str, link.TextToDisplay);
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
// Called: wb.Worksheets.Add("temp");
public void WorksheetCollection_Method_Add()
{
    Workbook wb = new Workbook();
    wb.Worksheets.Add("temp");
    Worksheet ws = wb.Worksheets["temp"];
    Aspose.Cells.Range range = ws.Cells.CreateRange("A10:R15");
    ws.Cells.AddRange(range);
          
    ws.Cells.DeleteRow(9);
    Assert.AreEqual(9, range.FirstRow);
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


