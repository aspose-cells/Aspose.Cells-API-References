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
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;

            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int index = tableStyles.AddTableStyle("CustomStyle1");
            TableStyle tableStyle = tableStyles[index];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            elements.Add(TableStyleElementType.FirstColumn);
            elements[0].SetElementStyle(firstColumnStyle);

            elements.Add(TableStyleElementType.LastColumn);
            elements[1].SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("Item2");
            cells["B3"].PutValue(200);

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.TableStyleName = "CustomStyle1";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;

            workbook.Save("TableStyleDemo.xlsx");
        }
    }
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

### See Also

* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


