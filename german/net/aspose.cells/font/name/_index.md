---
title: "Font.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt den Namen der Schrift zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/font/name/
---
## Font.Name property

Gibt den Namen des [`Font`](../) zurück oder legt ihn fest.

```csharp
public virtual string Name { get; set; }
```

### Hinweise

Wenn diese Eigenschaft verwendet wird, um den Namen der Schrift festzulegen, wird [`SchemeType`](../schemetype/) auf None aktualisiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das Standard-Arbeitsblatt und die Zellen zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Erstellen und ändern Sie einen Stil mit Schriftarteigenschaften
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Wende den Stil auf eine Zelle an
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


