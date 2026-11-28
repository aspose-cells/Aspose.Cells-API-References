---
title: "ReferredArea.StartColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea özelliği. Alanın başlangıç sütunu"
type: docs
url: /tr/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

Alanının başlangıç sütunu.

```csharp
public int StartColumn { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // B1:C2 aralığını referans alan bir adlandırılmış aralık oluşturun
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // Yeniden hesaplama false olarak ayarlandığında referans alanı al
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // StartColumn özelliğini gösterin
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // StartColumn kullanarak başvurulan alandaki değerleri yazdırın
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


