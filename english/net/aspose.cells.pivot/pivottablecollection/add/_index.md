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
// Called: int indPivTab = pivotTables.Add(sourceDataPT, "A2", "PivotTbl");
public void PivotTableCollection_Method_Add()
{
    LoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
    Workbook book = new Workbook(Constants.PivotTableSourcePath + "example.csv", loadOptions);
    book.Worksheets[0].Name = "LA_SUM";
    //Build Pivot table and Pivot Chart
    Aspose.Cells.Range rngAllData = book.Worksheets[0].Cells.MaxDisplayRange;
    Worksheet wsLASumPiv = book.Worksheets.Add("LA_SUM_Pivot");
    PivotTableCollection pivotTables = wsLASumPiv.PivotTables;
    string sourceDataPT = String.Format("=LA_SUM!{0}", rngAllData.Address);
    int indPivTab = pivotTables.Add(sourceDataPT, "A2", "PivotTbl");
    PivotTable pivotTable = pivotTables[indPivTab];

    int indSlicerYrs = wsLASumPiv.Slicers.Add(pivotTable, "E2", pivotTable.BaseFields["LA_Name"]);
    Slicer slicerYrs = wsLASumPiv.Slicers[indSlicerYrs];
    int indSlicerLA = wsLASumPiv.Slicers.Add(pivotTable, "E7", pivotTable.BaseFields["Year"]);
    Slicer slicerLA = wsLASumPiv.Slicers[indSlicerLA];

   Assert.AreEqual(4,slicerLA.SlicerCache.SlicerCacheItems.Count);
    book.Save(Constants.PivotTableDestPath + "example.xlsx");
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
// Called: var pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, 0, 0, "testPivot");
public void PivotTableCollection_Method_Add()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43717_";
    string savePath = CreateFolder(filePath);

    var dataSheetName = "data";
    var pivotSheetName = "pivot";
    var pivotDataRange = dataSheetName + "!A:C";

    var workbook = new Workbook(filePath + "PivotSortingTest.xlsx");
    var pivotWorksheet = workbook.Worksheets[pivotSheetName];
    var dataWorksheet = workbook.Worksheets[dataSheetName];

    var pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, 0, 0, "testPivot");
    var pivotTable = pivotWorksheet.PivotTables[pivotIndex];

    pivotTable.AddFieldToArea(PivotFieldType.Row, "Test1");

    pivotTable.AddFieldToArea(PivotFieldType.Data, "Test2");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Test3");
    pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

    pivotTable.DataFields["Test2"].Function = ConsolidationFunction.Sum;

    pivotTable.RowFields["Test1"].IsAutoSort = true;
    pivotTable.RowFields["Test1"].AutoSortField = 0;

    pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium8;

    dataWorksheet.IsVisible = false;

    pivotTable.RefreshData();
    pivotTable.CalculateData();

    Assert.AreEqual(pivotWorksheet.Cells["B4"].StringValue, "9");
    Assert.AreEqual(pivotWorksheet.Cells["B5"].StringValue, "9");
    Assert.AreEqual(pivotWorksheet.Cells["B6"].StringValue, "16");

    workbook.Save(savePath + "out.xlsx");

    PdfSaveOptions pdfOptions = new PdfSaveOptions();
    pdfOptions.AllColumnsInOnePagePerSheet = true;
    pdfOptions.CalculateFormula = true;

    workbook.Save(savePath + "out.pdf", pdfOptions);
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
public void PivotTableCollection_Method_Add()
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


