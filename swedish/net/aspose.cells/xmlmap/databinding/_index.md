---
title: "XmlMap.DataBinding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlMap property. Hämtar en XmlDataBinding för denna karta"
type: docs
url: /sv/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Hämtar en [`XmlDataBinding`](../../xmldatabinding/) av den här kartan.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempel på XML-kartor
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Lägg till första XML-kartan
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Lägg till andra XML-kartan
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Demonstrera användning av DataBinding‑egenskapen
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Spara arbetsboken
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Se även

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


