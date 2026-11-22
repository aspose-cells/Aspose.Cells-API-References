---
title: "DrawObjectEventHandler.Draw"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DrawObjectEventHandler. تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء العرض"
type: docs
url: /ar/net/aspose.cells.rendering/drawobjecteventhandler/draw/
---
## DrawObjectEventHandler.Draw method

تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير.

```csharp
public virtual void Draw(DrawObject drawObject, float x, float y, float width, float height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| drawObject | DrawObject | سيتم تهيئة DrawObject وإرجاعه أثناء العرض |
| x | Single | اليسار من DrawObject |
| y | Single | الجزء العلوي من DrawObject |
| العرض | Single | عرض DrawObject |
| الارتفاع | Single | ارتفاع DrawObject |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawObjectEventHandlerMethodDrawWithDrawObjectSingleSingleSingleSiDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells Drawing Demo";

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                sheetRender.ToImage(0, "DrawDemoOutput.png");
                Console.WriteLine("Draw method executed during rendering. Output saved to DrawDemoOutput.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }

        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // سيتم استدعاء هذا التنفيذ أثناء العرض لكل DrawObject
                Console.WriteLine($"Drawn {drawObject.Type} at ({x:F1}, {y:F1}) [{width:F1}x{height:F1}]");
            }
        }
    }
}
```

### انظر أيضًا

* class [DrawObject](../../drawobject/)
* class [DrawObjectEventHandler](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


