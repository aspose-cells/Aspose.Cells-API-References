---
title: "CellsHelper.DPI"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Makinenin DPI değerini alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Makinenin DPI değerini alır.

```csharp
public static double DPI { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Geçerli DPI'yi ayarla ve göster
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // DPI ayarını değiştir
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Yeni bir çalışma kitabı oluştur ve farklı DPI ayarlarıyla kaydet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // DPI etkisini göstermek için örnek bir şekil ekle
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Geçerli DPI ayarıyla kaydet
            workbook.Save("output_with_dpi_300.xlsx");

            // DPI'yi değiştir ve tekrar kaydet
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


