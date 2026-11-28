---
title: "HtmlTableLoadOption.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOption özelliği. HTML'den içe aktarılacak tablonun adını alın veya ayarlayın"
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

HTML'den içe aktarılacak tablonun adını alın veya ayarlayın

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection öğesine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Tablo indeksine göre yeni bir HtmlTableLoadOption ekleyin
            int index = tableLoadOptions.Add(0);

            // HtmlTableLoadOption öğesine erişin
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Name özelliğini ayarlayın
            option.Name = "CustomerDataTable";

            // Bir HTML dosyası yükleyin (gerçek dosya yolu ile değiştirin)
            workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


