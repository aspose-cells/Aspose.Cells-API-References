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
// Called: int pivotIndex = pivots.Add("=Sheet1!A1:C13", "A16", "TestPivotTable");
private PivotTable Method_String_(Workbook book)
        {
            Worksheet sheet = book.Worksheets[0];
            PivotTableCollection pivots = sheet.PivotTables;

            int pivotIndex = pivots.Add("=Sheet1!A1:C13", "A16", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            return pivot;
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
// Called: int pivotIndex = wsPivot.PivotTables.Add(dataRange.Name,
[Test]
        public void Method_String_()
        {
            Console.WriteLine("Method_String_()");
            string infn = path + "Test_PivotChart.xlsx";
            string outfn = Constants.destPath + "Test_PivotChart_out.xlsx";

            Workbook wb = new Workbook(infn);
            Worksheet wsPivot = wb.Worksheets["Pivot"];
            Worksheet wsData = wb.Worksheets["Data"];
            Aspose.Cells.Range dataRange = wsData.Cells.CreateRange(0, 0, 9, 6);
            dataRange.Name = "DataRange";

            int pivotIndex = wsPivot.PivotTables.Add(dataRange.Name,
                                0,
                                0,
                                "PivotTableAuto");
            PivotTable pivot = wsPivot.PivotTables[pivotIndex];
            for (int i = 0; i < pivot.BaseFields.Count; i++)
            {
                PivotField field = (PivotField)pivot.BaseFields[i];
                field.DisplayName = field.Name;
                field.IsAutoSubtotals = false;
                field.ShowInOutlineForm = true;
                field.ShowCompact = false;

                if (pivot.RowFields.Count < 1)
                {
                    pivot.AddFieldToArea(PivotFieldType.Row, field);
                    continue;
                }

                pivot.AddFieldToArea(PivotFieldType.Data, field);
            }

            pivot.AddFieldToArea(PivotFieldType.Column, pivot.DataField);
            pivot.IsAutoFormat = true;
            pivot.AutoFormatType = PivotTableAutoFormatType.Classic;
            pivot.ShowRowGrandTotals = false;
            pivot.DataField.ShowInOutlineForm = true;
            pivot.DataField.ShowCompact = false;

            int chartIx = wsPivot.Charts.Add(ChartType.Column, pivot.TableRange2.EndRow + 2, 0, pivot.TableRange2.EndRow + 20, pivot.TableRange2.EndColumn);
            Chart chart = wsPivot.Charts[chartIx];
            chart.PivotSource = wsPivot.Name + "!" + pivot.Name;

            wb.Save(outfn);
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
// Called: int pivotTableIndex = worksheet.PivotTables.Add("=A1:C133823", "J1", "PivotTable1",false,false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("a");
            cells["A1"].PutValue("b");
            cells["A1"].PutValue("c");
            for(int i = 1; i < 65535; i++)
            {
                cells[i, 0].PutValue(i);
                cells[i, 1].PutValue(i);
                cells[i, 2].PutValue(i);
            }
           
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a Pivot Table
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C133823", "J1", "PivotTable1",false,false);
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


