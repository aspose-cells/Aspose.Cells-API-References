---
title: "Workbook.CreateStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تنشئ نمطًا جديدًا"
type: docs
url: /ar/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

ينشئ نمطًا جديدًا.

```csharp
public Style CreateStyle()
```

### قيمة الإرجاع

تُرجع كائن نمط.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط جديد باستخدام طريقة CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // تعيين خصائص النمط
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // إنشاء علامة النمط وتعيين العلامات
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // تطبيق النمط على الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // ضبط العمود تلقائيًا
            worksheet.AutoFitColumn(0);
            
            // احفظ المصنف
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

ينشئ نمطًا جديدًا.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cloneDefaultStyle | منطقي | يشير إلى ما إذا كان ينسخ النمط الافتراضي |

### قيمة الإرجاع

تُرجع كائن نمط.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // إنشاء نمط جديد (false = عدم الوراثة من النمط الافتراضي)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // تطبيق النمط على خلية
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // احفظ المصنف
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


