---
title: PivotTableCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection method. Adds a new PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_5}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added cache index.

### Examples

```csharp
// Called: int pivotIndex = pivots.Add(&amp;quot;=Sheet1!A1:C5&amp;quot;, &amp;quot;A12&amp;quot;, &amp;quot;TestPivotTable&amp;quot;);
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;

            // Create date style
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = &quot;m/d/yyyy&quot;;
            cells[0, 1].Value = &quot;date&quot;;
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);

            // Set date style
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = &quot;amount&quot;;
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Add a PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C5&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;date&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Refresh PivotTable data
            pivot.RefreshData();
            pivot.CalculateData();

            // Add a Timeline to the worksheet
            TimelineCollection timelines = sheet.Timelines;
            int timelineIndex = timelines.Add(pivot, &quot;A20&quot;, &quot;date&quot;);

            // Access the added Timeline
            Timeline timeline = timelines[timelineIndex];

            // Save the workbook
            workbook.Save(&quot;TimelineCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_6}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added cache index.

### Examples

```csharp
// Called: PivotTable pt = ws.PivotTables[(ws.PivotTables.Add(&amp;quot;&amp;apos;Grid Results&amp;apos;!B4:E8&amp;quot;, 2, 0, &amp;quot;Hello&amp;quot;))];
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + &quot;SR3.xls&quot;);

            Worksheet ws = workbook.Worksheets[1];
            PivotTable pt = ws.PivotTables[(ws.PivotTables.Add(&quot;&apos;Grid Results&apos;!B4:E8&quot;, 2, 0, &quot;Hello&quot;))];
            pt.AddFieldToArea(PivotFieldType.Row, 1);
            pt.AddFieldToArea(PivotFieldType.Data, 0);
            pt.RowFields[0].IsAutoSort = true;
            workbook.Save(Constants.savePivottablePath + &quot;c.xls&quot;);
            //workbook.Save(&quot;D:\\c.xlsx&quot;, FileFormatType.Xlsx);
        }
```

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_4}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | Boolean | Indicates whether add classic pivot table of Excel 97-2003. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_7}

Adds a new PivotTable.

```csharp
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| cell | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | Boolean | Indicates whether add classic pivot table of Excel 97-2003. |

### Return Value

The new added cache index.

### Examples

```csharp
// Called: int pivotTableIndex = worksheet.PivotTables.Add(&amp;quot;=A1:C133823&amp;quot;, &amp;quot;J1&amp;quot;, &amp;quot;PivotTable1&amp;quot;,false,false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;a&quot;);
            cells[&quot;A1&quot;].PutValue(&quot;b&quot;);
            cells[&quot;A1&quot;].PutValue(&quot;c&quot;);
            for(int i = 1; i &lt; 65535; i++)
            {
                cells[i, 0].PutValue(i);
                cells[i, 1].PutValue(i);
                cells[i, 2].PutValue(i);
            }
           
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a Pivot Table
            int pivotTableIndex = worksheet.PivotTables.Add(&quot;=A1:C133823&quot;, &quot;J1&quot;, &quot;PivotTable1&quot;,false,false);
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Set the row fields
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Set the data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

         

        }
```

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Adds a new PivotTable based on another PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Adds a new PivotTable based on another PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_9}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_8}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | PivotPageFields | The pivot page field items. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


