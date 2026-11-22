---
title: "TableStyleElement.SetElementStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TableStyleElement. يضبط نمط العنصر"
type: docs
url: /ar/net/aspose.cells.tables/tablestyleelement/setelementstyle/
---
## TableStyleElement.SetElementStyle method

يضبط نمط العنصر.

```csharp
public void SetElementStyle(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | نمط العنصر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodSetElementStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.LightBlue;
            firstColumnStyle.Font.IsBold = true;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int index = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            index = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index];
            element.SetElementStyle(firstColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }

            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleElementMethodSetElementStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


