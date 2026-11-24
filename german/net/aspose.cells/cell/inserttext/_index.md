---
title: "Cell.InsertText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zellenmethode. Einige Zeichen in die Zelle einfügen. Wenn die Zelle reich formatiert ist, kann diese Methode die ursprüngliche Formatierung beibehalten"
type: docs
url: /de/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Fügt der Zelle einige Zeichen ein. Wenn die Zelle reich formatiert ist, kann diese Methode die ursprüngliche Formatierung beibehalten.

```csharp
public void InsertText(int index, string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index. |
| Text | String | Eingefügter Text. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zelle B3 zugreifen und Anfangswert festlegen
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Text an Position 6 einfügen
            cell.InsertText(6, "Inserted");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


