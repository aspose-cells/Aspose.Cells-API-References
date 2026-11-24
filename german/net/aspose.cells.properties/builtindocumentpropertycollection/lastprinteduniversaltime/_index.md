---
title: "BuiltInDocumentPropertyCollection.LastPrintedUniversalTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Liest oder setzt die universelle Zeit, zu der das Dokument zuletzt gedruckt wurde"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinteduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property

Liest oder setzt die universelle Zeit, zu der das Dokument zuletzt gedruckt wurde.

```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierten Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Setze die LastPrintedUniversalTime-Eigenschaft
            DateTime currentUtcTime = DateTime.UtcNow;
            builtInProperties.LastPrintedUniversalTime = currentUtcTime;

            // Zeige den gesetzten Wert an
            Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);

            // Speichere die Arbeitsmappe
            workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


