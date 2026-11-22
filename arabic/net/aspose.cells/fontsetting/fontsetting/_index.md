---
title: "FontSetting.FontSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ FontSetting."
type: docs
url: /ar/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 |  |
| الطول | Int32 |  |
| الأوراق | WorksheetCollection |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نص عينة إلى الخلية
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // إنشاء إعداد خط لأول 5 أحرف (0-4) في جميع أوراق العمل
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // تطبيق التنسيق
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


