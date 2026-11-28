---
title: "ReferredArea.StartRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea özelliği. Alanın başlangıç satırı"
type: docs
url: /tr/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

Alanının başlangıç satırı.

```csharp
public int StartRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı ve çalışma sayfası oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veri doldurun
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // A2:A4'e başvuran adlandırılmış bir aralık oluşturun
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // Yeniden hesaplama parametresiyle başvurulan alanı alın
            ReferredArea area = name.GetReferredAreas(false)[0];

            // StartRow özelliğini gösterin
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // StartRow ve EndRow kullanarak başvurulan alanı yineleyin
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


