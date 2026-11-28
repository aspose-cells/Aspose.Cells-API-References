---
title: "Enum DrawObjectEnum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.DrawObjectEnum enum. DrawObject'in Hücre veya Görüntü olduğunu belirtir"
type: docs
url: /tr/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

DrawObject'in Hücre ya da Görüntüsünü belirtir.

```csharp
public enum DrawObjectEnum
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Image | `0` | DrawObject'in bir Görüntü olduğunu belirtin |
| Cell | `1` | indicate DrawObject'in bir Hücre olduğunu belirtin |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // PdfSaveOptions nesnesi oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Özel bir DrawObjectEventHandler oluşturun
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Çalışma kitabını özel işleyici ile PDF olarak kaydedin
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Draw object'in bir hücre olup olmadığını kontrol edin
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Hücre bilgilerini çıktı olarak verin
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // A1 hücresi için özel işleme
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


