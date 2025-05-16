---
title: TableStyleElementCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TableStyleElementCollection property. Gets an element of the table style by the index
type: docs
url: /net/aspose.cells.tables/tablestyleelementcollection/item/
---
## TableStyleElementCollection indexer (1 of 2)

Gets an element of the table style by the index.

```csharp
public TableStyleElement this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

Returns [`TableStyleElement`](../../tablestyleelement/) object

### Examples

```csharp
// Called: element = elements[index1];
public static void TableStyleElementCollection_Property_Item()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create styles for the first and last columns
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Define a custom table style name
            string tableStyleName = "Custom1";

            // Access the table styles collection
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Add a new table style to the collection
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Access the table style elements collection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Add and configure the first column style element
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Add and configure the last column style element
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Populate the worksheet with sample data
            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a table to the worksheet
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Apply the custom table style to the table
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Save the workbook
            workbook.Save("TableStyleElementCollectionExample.xlsx");
        }
```

### See Also

* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleElementCollection indexer (2 of 2)

Gets the element of the table style by the element type.

```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```

| Parameter | Description |
| --- | --- |
| type | The element type. |

### Return Value

Returns [`TableStyleElement`](../../tablestyleelement/) object

### Examples

```csharp
namespace AsposeCellsExamples.TableStyleElementCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to create a table
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Create a table
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Get the table style from the workbook's table styles collection
            TableStyle tableStyle = workbook.Worksheets.TableStyles[table.TableStyleName];
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Access a specific table style element using indexer
            TableStyleElement firstRowElement = elements[TableStyleElementType.FirstRowStripe];
            Console.WriteLine("First row stripe element exists: " + (firstRowElement != null));

            // Add a new element if needed
            int newElementIndex = elements.Add(TableStyleElementType.FirstRowStripe);
            TableStyleElement newElement = elements[TableStyleElementType.FirstRowStripe];
            Console.WriteLine("New element added at index: " + newElementIndex);

            // Save the workbook
            workbook.Save("TableStyleElementCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


