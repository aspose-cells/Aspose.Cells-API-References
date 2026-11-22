---
title: "Cell.Replace"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. استبدال نص الخلية مع الخيارات"
type: docs
url: /ar/net/aspose.cells/cell/replace/
---
## Cell.Replace method

استبدال نص الخلية باستخدام الخيارات.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValue | String | قيمة السلسلة للاستبدال |
| خيارات | ReplaceOptions | خيارات الاستبدال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // إنشاء خيارات الاستبدال
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // احصل على إعدادات الخط من الخلية B1 لتطبيقها على الاستبدالات
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // استبدال جميع المتغيرات لـ "hello" بـ "Hi" باستخدام الخيارات
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


