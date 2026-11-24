---
title: "Enum SheetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SheetType-Enum. Gibt den Arbeitsblatttyp an"
type: docs
url: /de/net/aspose.cells/sheettype/
---
## SheetType enumeration

Gibt den Arbeitsblatttyp an.

```csharp
public enum SheetType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| VB | `0` | Visual Basic-Modul |
| Worksheet | `1` |  |
| Chart | `2` | Diagramm |
| BIFF4Macro | `3` | BIFF4-Makroblatt |
| InternationalMacro | `4` | Internationales Makroblatt |
| Other | `5` |  |
| Dialog | `6` | Dialog-Arbeitsblatt |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein neues Arbeitsblatt vom Typ Worksheet an Index 0 ein
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Legen Sie den Namen des neuen Arbeitsblatts fest
            newWorksheet.Name = "InsertedSheet";
            
            // Greifen Sie auf Zellen im neuen Arbeitsblatt zu und fügen Sie einige Daten hinzu
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Speichere die Arbeitsmappe
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


