---
title: TableStyleCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TableStyleCollection property. Gets the table style by the index
type: docs
url: /net/aspose.cells.tables/tablestylecollection/item/
---
## TableStyleCollection indexer (1 of 2)

Gets the table style by the index.

```csharp
public TableStyle this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The position of the table style in the list. |

### Return Value

The table style object.

### Examples

```csharp
// Called: TableStyle tableStyle = tableStyles[index1];
public static void TableStyleCollection_Property_Item()
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

* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleCollection indexer (2 of 2)

Gets the table style by the name.

```csharp
public TableStyle this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The table style name. |

### Return Value

The table style object.

### Examples

```csharp
namespace AsposeCellsExamples.TableStyleCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the table style collection from the workbook
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Add a new custom table style
            int index = tableStyles.AddTableStyle("CustomStyle1");
            TableStyle customStyle = tableStyles[index];

            // Set some properties of the custom style
            customStyle.TableStyleElements[TableStyleElementType.FirstRowStripe].GetElementStyle().Font.IsBold = true;

            // Access the style using Item property by name
            TableStyle retrievedStyle = tableStyles["CustomStyle1"];
            Console.WriteLine("Retrieved style name: " + retrievedStyle.Name);

            // Modify the retrieved style
            retrievedStyle.TableStyleElements[TableStyleElementType.FirstColumn].GetElementStyle().Font.Color = System.Drawing.Color.Red;

            // Create a table to demonstrate the style
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = "CustomStyle1";

            // Save the result
            workbook.Save("TableStyleCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


