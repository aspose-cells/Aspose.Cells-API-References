---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false'tur, bu yüzden boş satırın içeriği varsayılan olarak boş olur"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false olduğundan, boş satırın içeriği varsayılan olarak boş olur.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Boş satırlarla birlikte bazı veriler ekleyin
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // KeepSeparatorsForBlankRow true olarak ayarlanmış kaydetme seçenekleri oluştur
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Çalışma kitabını seçeneklerle CSV olarak kaydet
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
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


