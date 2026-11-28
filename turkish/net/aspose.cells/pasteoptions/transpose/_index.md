---
title: "PasteOptions.Transpose"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. Aralık yapıştırıldığında satır ve sütunları transpoze etmek için True. Varsayılan değer False"
type: docs
url: /tr/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

Aralık yapıştırıldığında satır ve sütunların yer değiştirmesi için True. Varsayılan değer False.

```csharp
public bool Transpose { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kaynak stili oluştur ve yatay aralığa uygula
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Transpozla yapıştırma seçenekleri oluştur
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Transpozla dikey aralığa kopyala
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


