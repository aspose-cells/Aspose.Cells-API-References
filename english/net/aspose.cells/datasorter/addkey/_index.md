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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sample data
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Add sort key for column B (index 1) with ascending order
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Sort data range (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Output sorted values
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sample data to sort
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Create data sorter and add custom sort key
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Sort the data
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Save the result
            workbook.Save("output.xlsx");
        }
    }
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
namespace AsposeCellsExamples
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

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


