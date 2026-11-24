---
title: "MetadataOptions.MetadataOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MetadataOptions Konstruktor. Erstellt eine Option zum Laden der Metadaten"
type: docs
url: /de/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Erstellt Optionen zum Laden der Metadaten.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| metadataType | MetadataType | Der Typ der Metadaten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Rufen Sie die #ctor-Methode mit dem Parameter MetadataType auf
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Zusätzliche Eigenschaften festlegen
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Anzeige der erstellten Optionen
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Verwenden Sie die Optionen beim Laden von Metadaten (Beispiel)
                // Dies würde typischerweise mit LoadOptions beim Öffnen einer Datei verwendet werden
                // Hinweis: Der ursprüngliche Code versuchte, MetadataOptions direkt auf LoadOptions zu setzen,
                // aber die LoadOptions-Klasse hat diese Eigenschaft in der bereitgestellten Definition nicht.
                // Wir behalten einfach den Teil zur Erstellung der Optionen, da die Verwendung mit LoadOptions
                // mit der aktuellen API-Definition nicht möglich ist.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Speichern Sie die Arbeitsmappe (obwohl Metadatenoptionen diese leere Arbeitsmappe nicht beeinflussen würden)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


