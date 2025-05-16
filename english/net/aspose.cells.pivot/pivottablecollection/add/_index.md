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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Define parameters for Add method
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Call the Add method with parameters (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Configure the pivot table
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Define the data range
            string sourceData = "A1:C4";
            
            try
            {
                // Call the Add method with parameters: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Access the newly created pivot table
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configure pivot table
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Define the source data range
            string sourceData = "A1:C5";

            try
            {
                // Call the Add method with parameters (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Configure the pivot table
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Save the result
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithPivotTableStringStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Create a pivot table from the data range
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Call the Add method with parameters (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Save the workbook to show the effect
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Create a source pivot table
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Call the Add method with parameters (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Save the workbook to show the effect
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Define data range
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Call the Add method with specified parameters
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Access the newly created pivot table
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configure pivot table fields
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Define parameters for Add method
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Call the Add method with specified parameters
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Configure the pivot table
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Refresh data
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


