---
title: "XmlMapCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo XmlMapCollection. Aggiungi un XmlMap tramite l'url/percorso di un file xml/xsd"
type: docs
url: /it/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Aggiungi un [`XmlMap`](../../xmlmap/) tramite l'url/percorso di un file xml/xsd.

```csharp
public int Add(string url)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| url | String | url/percorso di un file xml/xsd. |

### Valore di ritorno

[`XmlMap`](../../xmlmap/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Aggiungi mappe XML utilizzando lo schema e i file XML
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


