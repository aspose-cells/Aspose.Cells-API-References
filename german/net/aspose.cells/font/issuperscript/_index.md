---
title: "Font.IsSuperscript"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Schrift hochgestellt ist"
type: docs
url: /de/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift hochgestellt ist.

```csharp
public bool IsSuperscript { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Text zu Zelle A1 hinzu
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Formatieren Sie einen Teil des Textes als hochgestellt
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Überprüfen Sie die Hochstellungseinstellung
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


