---
title: "تعداد FontUnderlineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FontUnderlineType. يعدد أنواع تسطير الخط"
type: docs
url: /ar/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

يسرد أنواع تسطير الخط.

```csharp
public enum FontUnderlineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يمثل عدم وجود تسطير. |
| Single | `1` | يمثل تسطيرًا واحدًا. |
| Double | `2` | يمثل تسطيرًا مزدوجًا. |
| Accounting | `3` | يمثل تسطيرًا محاسبيًا واحدًا. |
| DoubleAccounting | `4` | يمثل تسطيرًا محاسبيًا مزدوجًا. |
| Dash | `5` | يمثل تسطيرًا متقطعًا |
| DashDotDotHeavy | `6` | يمثل تسطيرًا سميكًا من نوع Dash-Dot-Dot |
| DashDotHeavy | `7` | يمثل تسطيرًا سميكًا من نوع Dash-Dot |
| DashedHeavy | `8` | يمثل تسطيرًا سميكًا متقطعًا |
| DashLong | `9` | يمثل تسطيرًا طويلًا متقطعًا |
| DashLongHeavy | `10` | يمثل تسطيرًا سميكًا طويلًا متقطعًا |
| DotDash | `11` | يمثل تسطيرًا من نوع Dash-Dot |
| DotDotDash | `12` | يمثل تسطيرًا من نوع Dash-Dot-Dot |
| Dotted | `13` | يمثل تسطيرًا منقّطًا |
| DottedHeavy | `14` | يمثل تسطيرًا سميكًا منقّطًا |
| Heavy | `15` | يمثل تسطيرًا سميكًا |
| Wave | `16` | يمثل تسطيرًا متموجًا |
| WavyDouble | `17` | يمثل تسطيرًا متموجًا مزدوجًا |
| WavyHeavy | `18` | يمثل تسطيرًا متموجًا قويًا |
| Words | `19` | يمثل تسطير الأحرف غير الفارغة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية "A1" من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            
            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Hello Aspose!");

            // احصل على نمط الخلية
            Style style = cell.GetStyle();
            
            // عيّن نوع تسطير الخط إلى تسطير واحد
            style.Font.Underline = FontUnderlineType.Single;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


