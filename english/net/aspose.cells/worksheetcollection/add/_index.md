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
// Called: wb.Worksheets.Add();
[Test]
        public void Method_Add()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Name = &quot;Test1&quot;;
            wb.Worksheets.Add();
            wb.Worksheets[1].Copy(new Workbook(Constants.sourcePath + @&quot;Copy\N43200_590075.xml&quot;).Worksheets[0]);
            wb.Worksheets[1].Name = &quot;Test2&quot;;
            //Assert.AreEqual(&quot;=IF(Test1!$A$4=\&quot;\&quot;,0,2)&quot;, wb.Worksheets[1].Cells[&quot;A2&quot;].Formula, &quot;A2&apos;s formula in copied sheet&quot;);
            Assert.AreEqual(&quot;=IF(Test1!$A$4=\&quot;\&quot;,0,2)&quot;, wb.Worksheets[1].Cells[&quot;A2&quot;].Formula, &quot;A2&apos;s formula in copied sheet&quot;);
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
// Called: Worksheet sheet = wb.Worksheets.Add(&amp;quot;.special&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Worksheet sheet = wb.Worksheets.Add(&quot;.special&quot;);
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;a12345.b67890&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&quot; + sheet.Name + &quot;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;a12345.67890&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&quot; + sheet.Name + &quot;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;c.a12345.b67890&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&quot; + sheet.Name + &quot;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;c.a12345.b67890.d&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&quot; + sheet.Name + &quot;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;a12345.b67890.&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;, cell.Formula, sheet.Name);
            sheet.Name = &quot;a12345.b67890.a&quot;;
            cell.Formula = &quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;;
            Assert.AreEqual(&quot;=&apos;&quot; + sheet.Name + &quot;&apos;!A1&quot;, cell.Formula, sheet.Name);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


