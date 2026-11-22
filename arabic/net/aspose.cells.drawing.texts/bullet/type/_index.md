---
title: "Bullet.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Bullet. تحصل وتعيّن نوع الرصاصة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

يحصل على نوع bullet ويضبطه.

```csharp
public BulletType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مربع نص
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // تكوين خصائص الرصاصة
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // احفظ المصنف
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


