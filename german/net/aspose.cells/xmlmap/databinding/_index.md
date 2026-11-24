---
title: "XmlMap.DataBinding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlMap-Eigenschaft. Gibt ein XmlDataBinding dieser Karte zurück"
type: docs
url: /de/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Gibt ein [`XmlDataBinding`](../../xmldatabinding/) dieser Karte zurück.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Beispiel-XML-Karten hinzufügen
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Erste XML-Karte hinzufügen
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Zweiten XML-Map hinzufügen
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Verwendung der DataBinding-Eigenschaft demonstrieren
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Speichere die Arbeitsmappe
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


