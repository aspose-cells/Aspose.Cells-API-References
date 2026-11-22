---
title: "Cells.GetCellDisplayStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. احصل على نمط العرض للخلية المحددة"
type: docs
url: /ar/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

احصل على نمط العرض للخلية المعطاة.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية المحددة |
| عمود | Int32 | عمود الخلية المحددة |

### قيمة الإرجاع

نمط العرض للخلية المحددة.

### ملاحظات

نفس الشيء مع [`GetDisplayStyle`](../../cell/getdisplaystyle/)، ونفس الشيء عند استخدام SideBorders لـ `GetCellDisplayStyle`.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تحضير نمط cell للعرض
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // إنشاء نمط مخصص
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على cell
            cell.SetStyle(style);

            try
            {
                // استدعاء GetCellDisplayStyle مع الصف 0 والعمود 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // خصائص نمط العرض
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // تطبيق نمط العرض على خلية أخرى للتحقق البصري
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

احصل على نمط العرض للخلية المعطاة.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية المحددة |
| عمود | Int32 | عمود الخلية المحددة |
| adjacentBorders | BorderType | يشير إلى أي الحدود تحتاج إلى الفحص والتعديل وفقًا لحدود الخلايا المجاورة. يرجى الاطلاع على الوصف لنفس المعامل في [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### قيمة الإرجاع

نمط العرض للخلية المحددة.

### ملاحظات

إذا كان الخلية متأثرة أيضًا بإعدادات أخرى مثل التنسيق الشرطي، كائنات القوائم، إلخ، فقد يكون نمط العرض مختلفًا عن [`GetCellStyle`](../getcellstyle/). وبما أن هذه الإعدادات قد تُطبق أيضًا على الخلايا الفارغة (غير الموجودة)، فإن استخدام هذه الطريقة يمكن أن يتجنب إنشاء تلك الخلايا الفارغة لذا ستكون الأداء أفضل من الحصول على مثيل الخلية من Cells ثم استدعاء [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين نمط حد
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // استدعاء GetCellDisplayStyle مع معلمات محددة (0,0 للخلية A1، نوع TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // تحقق مما إذا كان النمط المسترجع يطابق لون الحد الخاص بنا
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // عرض تطبيق النمط عن طريق تعديل خلية أخرى
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


