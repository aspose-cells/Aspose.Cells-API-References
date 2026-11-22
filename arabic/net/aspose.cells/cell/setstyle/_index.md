---
title: "Cell.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تضبط نمط الخلية"
type: docs
url: /ar/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

يضبط نمط الخلية.

```csharp
public void SetStyle(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | نمط الخلية. |

### ملاحظات

إذا تم تغيير إعدادات الحدود، سيتم تحديث حدود الخلايا المعدلة أيضًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أنشئ نمطًا واضبط خصائصه
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // طبق النمط على الخلية B2 (1,1 في الفهرس الصفري)
            cells[1, 1].SetStyle(style);

            // احفظ المصنف
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

تطبيق الخاصية المعدلة للنمط على الخلية.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | نمط الخلية. |
| explicitFlag | منطقي | صحيح، فقط استبدال التنسيق الذي تم تعيينه صراحةً. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ الأنماط مباشرة
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // طبق الأنماط على الخلايا باستخدام طريقة SetStyle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // احفظ المصنف
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

تطبيق نمط الخلية بناءً على العلامات.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | نمط الخلية. |
| علامة | StyleFlag | علامة النمط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أنشئ نمطًا واضبط خصائصه
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // أنشئ علامة نمط واضبطها لتطبيق كل التنسيقات
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // احصل على الخلايا واضبط القيمة إلى A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // طبق النمط على الخلية باستخدام SetStyle
            cell.SetStyle(style, flag);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


