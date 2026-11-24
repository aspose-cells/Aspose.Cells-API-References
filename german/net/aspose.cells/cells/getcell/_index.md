---
title: "Cells.GetCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt das Cell-Element oder null am angegebenen Zeilen- und Spaltenindex zurück"
type: docs
url: /de/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Liefert das [`Cell`](../../cell/) Element oder null bei dem angegebenen Zeilen- und Spaltenindex der Zelle.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |
| column | Int32 | Spaltenindex |

### Rückgabewert

Gibt das Cell-Objekt zurück, wenn ein Cell-Objekt existiert. Gibt null zurück, wenn die Zelle nicht existiert.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode CheckCell(int row, int column). Diese Methode wird 12 Monate später, seit Februar 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die Zelle in Zeile 1, Spalte 2 zu (0-basierter Index).
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Wert und Stil für die Demonstration festlegen.
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


