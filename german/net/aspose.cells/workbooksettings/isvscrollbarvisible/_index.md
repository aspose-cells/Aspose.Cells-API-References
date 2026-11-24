---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält"
type: docs
url: /de/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Liest oder setzt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;
            
            // Vertikale Bildlaufleiste ausblenden
            settings.IsVScrollBarVisible = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


