---
title: "Cells.HideColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. إخفاء أعمدة متعددة"
type: docs
url: /ar/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

إخفاء أعمدة متعددة.

```csharp
public void HideColumns(int column, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| totalColumns | Int32 | رقم العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إخفاء الأعمدة من 3 إلى 5 (فهرس يبدأ من الصفر)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // احفظ المصنف
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


