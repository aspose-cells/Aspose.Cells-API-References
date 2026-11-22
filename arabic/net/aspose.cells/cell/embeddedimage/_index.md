---
title: "Cell.EmbeddedImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. الحصول على الصورة المدمجة في الخلية وتعيينها"
type: docs
url: /ar/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

يحصل على الصورة المدمجة في الخلية أو يضبطها.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // اختر خلية لتخزين الصورة المدمجة
                Cell cell = worksheet.Cells["B2"];

                // صورة PNG شفافة بحجم 1×1 بكسل (مشفرة Base64)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // تحويل سلسلة Base64 إلى مصفوفة بايت
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // تعيين الصورة المدمجة في الخلية
                cell.EmbeddedImage = imageBytes;

                // استرجاع الصورة المدمجة من الخلية
                byte[] retrievedBytes = cell.EmbeddedImage;

                // كتابة الصورة المسترجعة إلى ملف للتحقق من أنها تم تخزينها بشكل صحيح
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // حفظ المصنف (الصورة المدمجة مخزنة داخل ملف .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


