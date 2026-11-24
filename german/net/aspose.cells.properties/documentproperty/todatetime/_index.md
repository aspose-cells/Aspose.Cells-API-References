---
title: "DocumentProperty.ToDateTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Methode. Gibt den Eigenschaftswert als DateTime in der lokalen Zeitzone zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Gibt den Eigenschaftswert als DateTime in der lokalen Zeitzone zurück.

```csharp
public DateTime ToDateTime()
```

### Hinweise

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Date ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Abrufen der Sammlung benutzerdefinierter Dokumenteigenschaften
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Füge eine DateTime-Eigenschaft hinzu
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Rufe die Eigenschaft ab und konvertiere sie zu DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Gib das Ergebnis aus
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


