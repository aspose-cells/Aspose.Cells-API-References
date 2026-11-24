---
title: "Klasse VbaModule"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaModule-Klasse. Stellt das Modul im VBA-Projekt dar"
type: docs
url: /de/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Stellt das Modul im VBA‑Projekt dar.

```csharp
public class VbaModule
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Liest und schreibt die Binärcodes des Moduls. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Liest und schreibt die Codes des Moduls. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Liest und schreibt den Namen des Moduls. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Ermittelt den Typ des Moduls. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;

            // Ein neues Modul hinzufügen
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Das VBA-Modul abrufen
            VbaModule vbaModule = vbaProject.Modules[index];

            // Den Code für das Modul festlegen
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Die Excel-Datei speichern
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


