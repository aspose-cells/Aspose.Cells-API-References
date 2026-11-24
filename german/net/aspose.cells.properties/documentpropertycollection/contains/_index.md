---
title: "DocumentPropertyCollection.Contains"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentPropertyCollection-Methode. Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert"
type: docs
url: /de/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert.

```csharp
public bool Contains(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Groß-/Kleinschreibung‑unabhängige Name der Eigenschaft. |

### Rückgabewert

True, wenn die Eigenschaft in der Sammlung existiert; sonst false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Prüfe, ob die Eigenschaft "RevisionNumber" in den integrierten Dokumenteigenschaften existiert
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Füge eine benutzerdefinierte Eigenschaft hinzu und prüfe deren Vorhandensein
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Siehe auch

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


