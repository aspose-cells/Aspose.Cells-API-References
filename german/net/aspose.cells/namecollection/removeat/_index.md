---
title: "NameCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection‑Methode. Entfernt den Namen am angegebenen Index"
type: docs
url: /de/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Entfernt den Namen am spezifischen Index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Index des zu entfernenden Namens. |

### Hinweise

Bitte stellen Sie sicher, dass der Name nicht von anderen Formeln referenziert wird, bevor Sie die Methode aufrufen. Und wenn der Name referenziert wird, ist es besser, Name.RefersTo auf null zu setzen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Namen zur Sammlung hinzufügen
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Name nach Index entfernen
            names.RemoveAt(firstIndex);

            // Entfernung durch Überprüfung der Anzahl verifizieren
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


