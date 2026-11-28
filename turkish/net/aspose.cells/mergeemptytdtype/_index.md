---
title: "Enum MergeEmptyTdType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.MergeEmptyTdType enum. Boş bir TD öğesinin dosya HTML olarak dışa aktarılırken birleştirme türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Bir dosyayı HTML'ye dışa aktarırken boş TD öğesi için birleştirme türünü temsil eder.

```csharp
public enum MergeEmptyTdType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | MS Excel gibi görüntüle. |
| None | `1` | Boş TD öğeleri dosya HTML olarak dışa aktarılırken birleştirilmeyecek. Bu, önemli ölçüde daha büyük bir HTML dosyası oluşturacaktır. |
| MergeForcely | `2` | Dosya HTML olarak dışa aktarılırken boş TD öğesi zorunlu olarak birleştiriliyor. Değer true olarak ayarlandığında HTML dosyasının boyutu önemli ölçüde azalacaktır. HTML dosyasını Excel'e içe aktarmak veya dosyayı HTML olarak kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // HtmlSaveOptions oluşturun ve MergeEmptyTdType özelliğini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


