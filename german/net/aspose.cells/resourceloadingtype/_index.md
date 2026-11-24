---
title: "Enum ResourceLoadingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ResourceLoadingType-Enum. Stellt dar, wie die verknüpfte Ressource geladen wird"
type: docs
url: /de/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Stellt dar, wie die verknüpfte Ressource geladen wird.

```csharp
public enum ResourceLoadingType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Lädt diese Ressource wie üblich. |
| Skip | `1` | Überspringt das Laden dieser Ressource. |
| UserProvided | `2` | Verwenden Sie den vom Benutzer bereitgestellten Stream |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Speichern Sie die Arbeitsmappe als HTML mit benutzerdefiniertem Stream-Anbieter
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Stellen Sie einen benutzerdefinierten Stream für die Ressource bereit
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Laden der Ressource überspringen
                options.Stream = Stream.Null;
            }
            else
            {
                // Laden Sie die Ressource wie üblich
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Schließe den Stream, wenn er nicht null ist
            options.Stream?.Close();
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


