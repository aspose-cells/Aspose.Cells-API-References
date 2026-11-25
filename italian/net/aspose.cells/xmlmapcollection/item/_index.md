---
title: "XmlMapCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlMapCollection. Ottiene la mappa xml per l'indice specifico"
type: docs
url: /it/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Ottiene la mappa xml per l'indice specificato.

```csharp
public XmlMap this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La mappa xml

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi a XmlMapCollection dal workbook
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Aggiungi un nuovo XmlMap alla raccolta
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Accedi all'XmlMap utilizzando la proprietà Item
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Visualizza il nome dell'XmlMap
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Salva la cartella di lavoro
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


