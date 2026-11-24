---
title: "NameCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection‑Methode. Definiert einen neuen Namen"
type: docs
url: /de/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Definiert einen neuen Namen.

```csharp
public int Add(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text, der als Name verwendet werden soll. |

### Rückgabewert

[`Name`](../../name/) object index.

### Hinweise

Der Name darf keine Leerzeichen enthalten und darf nicht wie Zellreferenzen aussehen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Fügen Sie einen Namen mit Zeichenkettenreferenz hinzu
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Legen Sie die Formel fest, auf die sich der Name bezieht
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Überprüfen und die Ergebnisse ausgeben
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Holen Sie den Bereich und zeigen Sie dessen Adresse an
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


