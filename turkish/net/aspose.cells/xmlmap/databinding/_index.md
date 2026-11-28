---
title: "XmlMap.DataBinding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlMap özelliği. Bu haritanın bir XmlDataBinding'ini alır"
type: docs
url: /tr/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Bu haritanın bir [`XmlDataBinding`](../../xmldatabinding/) alır.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek XML haritaları ekle
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // İlk XML haritasını ekle
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // İkinci XML haritasını ekle
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // DataBinding özelliğinin kullanımını göster
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Çalışma kitabını kaydedin
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


