---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOption özelliği. İçe aktarılan tablodan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

İçe aktarılan tablodan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool TableToListObject { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // TableToListObject etkinleştirilmiş HTML yükleme seçeneklerini oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Belirtilen seçeneklerle HTML'yi yükleyin
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


