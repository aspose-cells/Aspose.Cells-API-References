---
title: "XmlMap.DataBinding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlMap. Ottiene un XmlDataBinding di questa mappa"
type: docs
url: /it/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Ottiene un [`XmlDataBinding`](../../xmldatabinding/) di questa mappa.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi mappe XML di esempio
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Aggiungi la prima mappa XML
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Aggiungi la seconda mappa XML
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Dimostra l'uso della proprietà DataBinding
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Salva la cartella di lavoro
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


