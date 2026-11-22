---
title: "MsoFillFormatHelper.Texture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormatHelper. يحصل على نوع تعبئة القوام"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

الحصول على نوع ملء النسيج.

```csharp
public TextureType Texture { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تسمية لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // أنشئ مثيلًا لـ MsoFillFormatHelper باستخدام الانعكاس (بدون مُنشئ عام)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // اعرض القيمة الحالية لخاصية Texture (للقراءة فقط)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // أظهر أن الخاصية للقراءة فقط بمحاولة تعيينها (مُعلّق)
                // fillHelper.Texture = TextureType.Canvas; // سيؤدي هذا إلى خطأ في التجميع

                // اعرض جميع أنواع القوام المتاحة للمرجع
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // احفظ المصنف لعرض التنفيذ الناجح
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


