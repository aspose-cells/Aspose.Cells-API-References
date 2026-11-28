---
title: "Sınıf HtmlTableLoadOption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlTableLoadOption sınıfı. HTML'den tablo içe aktarıldığında seçeneği temsil eder."
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

HTML'den tablo içe aktarılırken seçeneği temsil eder.

```csharp
public class HtmlTableLoadOption
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | HTML'den içe aktarılacak tablonun kimliğini alın veya ayarlayın |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) HTML'den içe aktarılacak tablonun adını alın veya ayarlayın |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | HTML'deki çalışma sayfasının orijinal indeksini alın veya ayarlayın. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | HTML'den içe aktarılacak tablonun indeksini alın veya ayarlayın. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | İçe aktarılan tablodan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Tablonun yer alacağı çalışma sayfasının hedef indeksini alın veya ayarlayın. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // HtmlLoadOptions bir örnek oluştur.
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOption sınıfının bir örneğini oluşturun
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // HtmlTableLoadOption'ı HtmlLoadOptions'a ekleyin
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Belirtilen yükleme seçenekleriyle HTML dosyasını çalışma kitabına yükleyin
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


