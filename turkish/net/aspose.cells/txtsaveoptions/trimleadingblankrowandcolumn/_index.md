---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Başlangıçtaki boş satır ve sütunların, ms excel'in yaptığı gibi kırpılıp kırpılmayacağını gösterir. Varsayılan değer true'tir"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

ms excel'in yaptığı gibi baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. Varsayılan değer true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Açıklamalar

ms excel'deki kuralla aynı şekilde, bir satır/sütun özel stil içeriyorsa, hücre verisi olmasa bile boş olarak kabul edilmez. LightCells modunda kaydederken bu seçenek etkili olmaz. Kullanıcı, çıktının kapsamını [`LightCellsDataProvider`](../lightcellsdataprovider/) uygulamasıyla ya da [`ExportArea`](../exportarea/) belirterek kontrol etmelidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Bazı veri ve boş satır/sütun içeren örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Başlangıçta boş satır ve sütunlarla bazı veri ekle
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Başlangıçtaki boşlukları kırpmadan kaydet
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Başlangıçtaki boşlukları kırparak kaydet
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


