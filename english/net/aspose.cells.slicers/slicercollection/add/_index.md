---
title: SlicerCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SlicerCollection method. Add a new Slicer using PivotTable as data source
type: docs
url: /net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Add slicer
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Add pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Add slicer for the pivot table
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Create pivot table
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Add slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Create pivot table
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Add pivot fields
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Add slicer
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Save the workbook
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Create pivot table
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Add slicer
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Save the workbook
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | Int32 | The index of ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create sample data and list object
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Add slicer for the list object - note: Slicers.Add returns int index
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Save the workbook
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


