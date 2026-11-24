---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Ruft die universelle Zeit des letzten Speichervorgangs ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Liest oder setzt die universelle Zeit der letzten Speicherung.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Hinweise

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierten Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Setzen Sie die LastSavedUniversalTime-Eigenschaft
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Zeige den gesetzten Wert an
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Speichere die Arbeitsmappe
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


