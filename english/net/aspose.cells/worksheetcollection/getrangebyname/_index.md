---
title: WorksheetCollection.GetRangeByName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets Range object by predefined name
type: docs
url: /net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Gets Range object by pre-defined name.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

### Return Value

Range object.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range range = wb.Worksheets.GetRangeByName(rangeName);
private Aspose.Cells.Range WorksheetCollection_Method_GetRangeByName(Workbook wb, string rangeName, bool throwIfNotFound)
        {
            Aspose.Cells.Range range = wb.Worksheets.GetRangeByName(rangeName);
            if (range == null && throwIfNotFound)
            {
                throw new ApplicationException(string.Format("No range exists with name '{0}'", rangeName));
            }

            return range;
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Gets [`Range`](../../range/) by pre-defined name or table's name

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Int32 | The sheet index. -1 represents global . |
| includeTable | Boolean | Indicates whether checking all tables. |

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a named range
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Add some data to the range
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Call GetRangeByName with parameters (String, Int32, Boolean)
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Display range values
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


