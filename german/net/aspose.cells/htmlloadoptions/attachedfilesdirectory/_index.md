---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Das Verzeichnis, in dem die angehängten Dateien gespeichert werden"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

Das Verzeichnis, in dem die angehängten Dateien gespeichert werden.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die HtmlLoadOptions.StreamProvider-Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Dezember 2014, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Verzeichnis für angehängte Dateien festlegen
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Laden Sie eine HTML-Datei in ein Arbeitsbuch mit den angegebenen Optionen
            Workbook workbook = new Workbook("input.html", options);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


