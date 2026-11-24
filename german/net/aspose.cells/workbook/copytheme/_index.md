---
title: "Workbook.CopyTheme"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Kopiert das Design aus einer anderen Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Kopiert das Design aus einer anderen Arbeitsmappe.

```csharp
public void CopyTheme(Workbook source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Arbeitsmappe | Quellarbeitsmappe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Quellarbeitsmappe erstellen (Design wird automatisch gesetzt, wenn eine Vorlagendatei geöffnet wird)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            
            // Design von der Quell- zur Zielarbeitsmappe kopieren
            destWorkbook.CopyTheme(sourceWorkbook);

            // Speichere das Zielarbeitsbuch
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


