---
title: "SmartTagCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SmartTagCollection. Aggiunge un tag intelligente"
type: docs
url: /it/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Aggiunge un tag intelligente.

```csharp
public int Add(string uri, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uri | String | Specifica l'URI dello spazio dei nomi del tag intelligente |
| name | String | Specifica il nome del tag intelligente. |

### Valore di ritorno

L'indice dello smart tag nell'elenco.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


