---
title: "CellArea.EndColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حقل CellArea. يحصل أو يضبط العمود النهائي لهذا النطاق"
type: docs
url: /ar/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

يحصل أو يضبط العمود النهائي لهذه المساحة.

```csharp
public int EndColumn;
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء نطاق خلايا من A1 إلى C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // معالجة نطاق الخلايا باستخدام EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // احفظ المصنف
            workbook.Save("CellAreaFieldEndColumnDemo_output.xlsx");
        }

        private static void ProcessCellArea(CellArea area, Color color, Worksheet sheet)
        {
            int k = 0;
            for (int col = area.StartColumn; col <= area.EndColumn; col++)
            {
                for (int row = area.StartRow; row <= area.EndRow; row++)
                {
                    Cell cell = sheet.Cells[row, col];
                    
                    if (!color.IsEmpty)
                    {
                        Style style = cell.GetStyle();
                        style.ForegroundColor = color;
                        style.Pattern = BackgroundType.Solid;
                        cell.SetStyle(style);
                    }
                    
                    cell.PutValue(row + col + k);
                    k++;
                }
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


