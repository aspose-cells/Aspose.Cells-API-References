---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. QuotePrefix true olduğunda tek tırnak işaretinin bir hücrenin değerinin bir parçası olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

`QuotePrefix`(../../style/quoteprefix/) true olduğunda tek tırnak işaretinin bir hücrenin değerinin bir parçası olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportQuotePrefixDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Özel karakterlerle örnek veri ekle
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // TXT kaydetme seçenekleri oluştur
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // ExportQuotePrefix = true ile kaydet
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // Ayırıcıyı değiştir ve tekrar kaydet
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


