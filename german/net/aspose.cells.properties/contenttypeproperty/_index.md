---
title: "Klasse ContentTypeProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.ContentTypeProperty‑Klasse. Stellt Identifikationsinformationen dar"
type: docs
url: /de/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Stellt Identifikatorinformationen dar.

```csharp
public class ContentTypeProperty
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Gibt an, ob der Wert leer sein könnte. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Gibt den Namen des Objekts zurück oder setzt ihn. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Liest und setzt den Typ der Eigenschaft. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Gibt den Wert der Content‑Typ‑Eigenschaft zurück oder setzt ihn. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Eine neue Content‑Typ‑Eigenschaft hinzufügen
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Zugriff auf die neu hinzugefügte Eigenschaft
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Eigenschaften festlegen
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Speichere die Excel-Datei
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


