---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOptionCollection özelliği. Belirtilen indeksteki HtmlTableLoadOption öğesini alır"
type: docs
url: /tr/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Belirtilen indeksteki [`HtmlTableLoadOption`](../../htmltableloadoption/) öğesini alır.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Tablo indeksine göre yeni bir HtmlTableLoadOption ekleyin
            int index1 = tableLoadOptions.Add(0);

            // Item özelliğini kullanarak HtmlTableLoadOption öğesine erişin
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Tablo yükleme seçeneğini yapılandırın
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Yapılandırılmış seçeneklerle HTML dosyasını yükle
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


