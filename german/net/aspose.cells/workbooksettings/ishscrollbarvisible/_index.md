---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält."
type: docs
url: /de/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Liest oder setzt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;
            
            // Verstecke die horizontale Bildlaufleiste.
            settings.IsHScrollBarVisible = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


