---
title: "XmlDataBinding.Url"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlDataBinding özelliği. Bu veri bağlamasının kaynak URL'sini alır"
type: docs
url: /tr/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Bu veri bağlamanın kaynak url'sini alır.

```csharp
public string Url { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İki çalışma sayfası ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Liste nesneleri ve XML haritaları ekle
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // XML veri bağlama URL'lerini al (Url yalnızca okunur)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // URL'leri göster
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Çalışma kitabını kaydedin
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


