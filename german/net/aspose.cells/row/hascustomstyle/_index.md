---
title: "Row.HasCustomStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat, die sich vom standardmäßig vom Arbeitsbuch geerbten unterscheiden"
type: docs
url: /de/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat (anders als die standardmäßige, die vom Arbeitsbuch geerbt wird).

```csharp
public bool HasCustomStyle { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle und passe einen Stil an
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Greifen Sie auf die erste Zeile zu
            Row row = worksheet.Cells.Rows[0];
            
            // Wende den benutzerdefinierten Stil auf die Zeile an
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Überprüfe, ob die Zeile einen benutzerdefinierten Stil hat (sollte wahr sein)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


