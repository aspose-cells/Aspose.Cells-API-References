---
title: "XmlMap.RootElementName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlMap. Ottiene il nome dell'elemento radice"
type: docs
url: /it/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Ottiene il nome dell'elemento radice.

```csharp
public string RootElementName { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Crea una mappa XML
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // Ottieni e visualizza il nome dell'elemento radice
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### Vedi anche

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


