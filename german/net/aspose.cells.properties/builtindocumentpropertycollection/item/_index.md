---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Gibt ein DocumentProperty-Objekt anhand des Namens der Eigenschaft zurück"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Gibt ein [`DocumentProperty`](../../documentproperty/)‑Objekt anhand des Namens der Eigenschaft zurück.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Groß-/Kleinschreibung‑unabhängige Name der abzurufenden Eigenschaft. |

### Hinweise

Die Zeichenkettennamen der Eigenschaften entsprechen den Namen der typisierten Eigenschaften, die von [`BuiltInDocumentPropertyCollection`](../) verfügbar sind.

Wenn Sie eine Eigenschaft anfordern, die im Dokument nicht vorhanden ist, deren Name jedoch als gültiger integrierter Name erkannt wird, wird ein neues [`DocumentProperty`](../../documentproperty/) erstellt, zur Sammlung hinzugefügt und zurückgegeben. Der neu erstellten Eigenschaft wird ein Standardwert zugewiesen (leere Zeichenkette, Null, false oder DateTime.MinValue, abhängig vom Typ der integrierten Eigenschaft).

Wenn Sie eine Eigenschaft anfordern, die im Dokument nicht vorhanden ist und deren Name nicht als integrierter Name erkannt wird, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze eine integrierte Dokumenteigenschaft mit der richtigen Methode
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Greife auf den Eigenschaftswert zu und gib ihn aus
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe und überprüfe die Eigenschaft
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


