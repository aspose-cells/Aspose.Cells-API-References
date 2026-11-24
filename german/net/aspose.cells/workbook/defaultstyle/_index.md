---
title: "Workbook.DefaultStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Ruft das Standard-Style-Objekt des Workbooks ab oder legt es fest"
type: docs
url: /de/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Ruft das Standard-`[`Style`](../../style/)`-Objekt des Workbooks ab oder legt es fest.

```csharp
public Style DefaultStyle { get; set; }
```

### Hinweise

Die DefaultStyle‑Eigenschaft ist nützlich, um einen Style für das gesamte Workbook zu implementieren.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Hole den Standardstil und ändere seine Schriftart
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Wende den modifizierten Stil wieder als Standard an
            workbook.DefaultStyle = defaultStyle;
            
            // Erstelle ein Arbeitsblatt und füge etwas Text mit dem Standardstil hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Speichere die Arbeitsmappe
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


