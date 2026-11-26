---
title: "PdfSaveOptions.SetImageResample"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PdfSaveOptions. Устанавливает желаемое количество PPIpixels на дюйм для ресэмплинга изображений и качество jpeg. Все изображения будут преобразованы в JPEG с указанным качеством, а изображения, превышающие заданное количество PPIpixels на дюйм, будут ресэмплированы"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Устанавливает желаемое PPI (pixels per inch) для ресемплинга изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным параметром качества, и изображения, у которых PPI превышает указанное значение (pixels per inch), будут ресемплированы.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredPPI | Int32 | Желаемое количество пикселей на дюйм. 220 — высокое качество. 150 — качество для экрана. 96 — качество для электронной почты. |
| jpegQuality | Int32 | 0 – 100 % качества JPEG. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("Book1.xlsx");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SetImageResample(96, 80);
            
            wb.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


