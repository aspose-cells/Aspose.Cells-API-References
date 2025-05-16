---
title: DataSorter.AddKey
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Adds sorted column index and sort order
type: docs
url: /net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Adds sorted column index and sort order.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order |

### Examples

```csharp
// Called: workbook.DataSorter.AddKey(5, SortOrder.Ascending);
// Does Aspose.Cells have ability to add sort fields to ListObjects
// http://www.aspose.com/community/forums/thread/292632.aspx
public void DataSorter_Method_AddKey()
{
    Console.WriteLine("DataSorter_Method_AddKey()");
    string infn = path + @"ListObjectSort\ListObjectSort.xlsx";
    string outfn = Constants.destPath + @"ListObjectSort_out.xlsx";

    Workbook workbook = new Workbook(infn);
    workbook.DataSorter.AddKey(5, SortOrder.Ascending);
    workbook.DataSorter.Sort(workbook.Worksheets[0].Cells, 4, 3, 6, 5);
    Assert.LessOrEqual(workbook.Worksheets[0].Cells["F5"].IntValue,
        workbook.Worksheets[0].Cells["F6"].IntValue);
    Assert.LessOrEqual(workbook.Worksheets[0].Cells["F6"].IntValue,
        workbook.Worksheets[0].Cells["F7"].IntValue);
    workbook.Save(outfn, SaveFormat.Xlsx);
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order. |
| customList | String | The custom sort list. |

### Examples

```csharp
// Called: sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
public void DataSorter_Method_AddKey()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Sort/File_for_CustomSort_ASPOSE_Forum_Question.xlsx");
    DataSorter sorter = workbook.DataSorter;
    sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
    sorter.HasHeaders = true;
    sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A1", "C23"));
    Cells cells = workbook.Worksheets[1].Cells;
    Assert.AreEqual(cells["A2"].StringValue, "aaa");
    Assert.AreEqual(cells["A7"].StringValue, "ddd");
    Assert.AreEqual(cells["A12"].StringValue, "ccc");
    Assert.AreEqual(cells["A18"].StringValue, "bbb");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | SortOnType | The sorted value type. |
| order | SortOrder | The sort order. |
| customList | Object | The custom sort list. |

### Remarks

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

### Examples

```csharp
namespace AsposeCellsExamples.DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Create a data sorter
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Call AddKey with parameters: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Define the range to sort
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Sort the data
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Save the result
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### See Also

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order. |
| customList | String[] | The custom sort list. |

### Examples

```csharp
namespace AsposeCellsExamples.DataSorterMethodAddKeyWithInt32SortOrderStringDemo
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Department");
            worksheet.Cells["C1"].PutValue("Salary");
            
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue("HR");
            worksheet.Cells["C2"].PutValue(5000);
            
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("IT");
            worksheet.Cells["C3"].PutValue(6000);
            
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("HR");
            worksheet.Cells["C4"].PutValue(4500);
            
            worksheet.Cells["A5"].PutValue("Eve");
            worksheet.Cells["B5"].PutValue("IT");
            worksheet.Cells["C5"].PutValue(5500);

            // Create data sorter
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            // Define custom sort order for Department column
            string[] customOrder = { "IT", "HR" };

            try
            {
                // Add sort key for Department column (column index 1) with custom order
                sorter.AddKey(1, SortOrder.Ascending, customOrder);
                
                // Add secondary sort key for Salary column (column index 2)
                sorter.AddKey(2, SortOrder.Descending);

                // Sort data range
                sorter.Sort(worksheet.Cells, 0, 0, 5, 2);

                Console.WriteLine("Data sorted successfully with custom order for Department column");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOrderStringDemo.xlsx");
        }
    }
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


