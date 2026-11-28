---
title: "HtmlTableLoadOption.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOption özelliği. HTML'den içe aktarılacak tablonun kimliğini al veya ayarla"
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

HTML'den içe aktarılacak tablonun kimliğini alın veya ayarlayın

```csharp
public string Id { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tablo yükleme seçeneklerini yapılandır
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Tablo yükleme seçenekleri ekle
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Belirtilen seçeneklerle HTML dosyasını yükle
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


