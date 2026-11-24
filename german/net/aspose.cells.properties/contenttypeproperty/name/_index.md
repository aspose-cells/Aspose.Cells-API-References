---
title: "ContentTypeProperty.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypeProperty-Eigenschaft. Gibt den Namen des Objekts zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Gibt den Namen des Objekts zurück oder setzt ihn.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Eine Inhaltstyp-Eigenschaft mit dem Namen "ss" hinzufügen
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Im XLS-Format speichern
            workbook.Save("example.xls");
            
            // Arbeitsmappe neu laden und die Name-Eigenschaft überprüfen
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Im XLSX-Format speichern
            workbook.Save("example.xlsx");
            
            // Neu laden und erneut überprüfen
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Siehe auch

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


