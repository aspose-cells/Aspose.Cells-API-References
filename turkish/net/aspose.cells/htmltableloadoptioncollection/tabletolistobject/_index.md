---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOptionCollection özelliği. İçe aktarılan tablolardan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

İçe aktarılan tablolardan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false.

```csharp
public bool TableToListObject { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection örneğine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // HTML tablolarını ListObject'lere dönüştürmek için TableToListObject özelliğini ayarlayın.
            tableLoadOptions.TableToListObject = true;

            // İndeksle ListObject'e dönüştürülecek bir tablo ekleyin.
            tableLoadOptions.Add(0);

            // Yükleme seçeneklerini kullanarak bir HTML dosyasını çalışma kitabına yükleyin
            workbook = new Workbook("input.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


