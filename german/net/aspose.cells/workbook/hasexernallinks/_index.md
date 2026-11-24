---
title: "Workbook.HasExernalLinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Gibt an, ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält"
type: docs
url: /de/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Gibt an, ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Rückgabewert

Ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen ExternalLinkCollection.Count, um zu prüfen, ob in dieser Arbeitsmappe externe Verknüpfungen vorhanden sind. Diese Methode wird 12 Monate später, seit Dezember 2021, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit externen Verknüpfungen
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine externe Verknüpfung hinzu
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Überprüfen Sie, ob die Arbeitsmappe externe Verknüpfungen hat
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


