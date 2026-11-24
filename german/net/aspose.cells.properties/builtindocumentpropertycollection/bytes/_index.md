---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Stellt eine Schätzung der Anzahl von Bytes im Dokument dar"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

Stellt eine Schätzung der Anzahl von Bytes im Dokument dar.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Aktuellen Bytes-Wert anzeigen (Schätzung der Dokumentgröße)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // Fügen Sie etwas Inhalt hinzu, um die Größe zu beeinflussen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // Aktualisieren Sie die Bytes-Eigenschaft manuell (obwohl sie normalerweise automatisch berechnet wird)
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // Speichern Sie die Arbeitsmappe, um die Eigenschaft in der gespeicherten Datei zu sehen
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


