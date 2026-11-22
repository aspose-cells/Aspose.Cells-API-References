---
title: "BorderCollection.DiagonalColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BorderCollection. تحصل أو تعين لون الخطوط القطرية"
type: docs
url: /ar/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

يحصل أو يضبط Color للخطوط القطرية.

```csharp
public Color DiagonalColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // تعيين خصائص الحد القطري
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


