---
title: "XmlMap.DataBinding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlMap. Obtient un XmlDataBinding de ce mappage."
type: docs
url: /fr/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Obtient un [`XmlDataBinding`](../../xmldatabinding/) de ce mappage.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des cartes XML d'exemple
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Ajouter la première carte XML
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Ajouter la deuxième carte XML
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Démontrer l’utilisation de la propriété DataBinding
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Enregistrez le classeur
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


