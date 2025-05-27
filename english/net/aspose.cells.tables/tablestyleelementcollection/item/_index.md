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
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Pattern = BackgroundType.Solid;
            firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data");

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = styleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo2
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


