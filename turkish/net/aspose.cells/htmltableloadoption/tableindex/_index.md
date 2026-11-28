---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOption özelliği. HTML'den içe aktarılacak tablonun indeksini alın veya ayarlayın"
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

HTML'den içe aktarılacak tablonun indeksini alın veya ayarlayın.

```csharp
public int TableIndex { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // TableIndex = 0 (ilk tablo) ile tablo yükleme seçeneğini yapılandırın
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Tablo yükleme seçeneğini ekleyin
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // HTML dosyasını yükleyin (gerçek yol ile değiştirin)
            workbook = new Workbook("input.html", loadOptions);

            // Excel dosyası olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


