---
title: "Cells.ClearFormats"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تمسح تنسيق نطاق"
type: docs
url: /ar/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

يمسح تنسيق نطاق.

```csharp
public void ClearFormats(CellArea range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | CellArea | النطاق الذي سيُمسح. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات عينة مع تنسيق
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // تطبيق التنسيق على الخلايا
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // تحديد منطقة مسح
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // مسح التنسيقات من الخلية المركزية
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // تحديث قيمة الخلية الممسوحة لإظهار التأثير
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

يمسح تنسيق نطاق.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| endColumn | Int32 | فهرس العمود النهائي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تطبيق الأنماط على بعض الخلايا
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // مسح التنسيقات من نطاق محدد (الصفوف 5-15، الأعمدة 5-15)
            cells.ClearFormats(5, 5, 15, 15);

            // احفظ المصنف
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


