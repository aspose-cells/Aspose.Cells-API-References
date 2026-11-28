---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan değer false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Açıklamalar

LightCells modunda kaydederken ve [`ExportArea`](../exportarea/) belirtilmemişse, bu seçenek etkisiz olur ve bir satır, uygulamanın sağladığı son hücreye kadar genişletilir [`LightCellsDataProvider`](../lightcellsdataprovider/)

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Örnek veri ekleyin.
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Sondaki boş hücreleri kırpmadan kaydet (varsayılan)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Sondaki boş hücreleri kırparak kaydet
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


