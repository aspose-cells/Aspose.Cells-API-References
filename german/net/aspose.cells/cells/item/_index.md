---
title: "Cells.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt das Cell-Element am angegebenen Zeilen‑ und Spaltenindex zurück."
type: docs
url: /de/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Gibt das [`Cell`](../../cell/)‑Element am angegebenen Zeilen‑ und Spaltenindex zurück.

```csharp
public Cell this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Zeilenindex. |
| column | Spaltenindex. |

### Rückgabewert

Das [`Cell`](../../cell/)‑Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Verwenden der Item‑Eigenschaft zum Zugriff und zur Modifikation von Zellen
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Verwenden der Style‑Eigenschaft über Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Speichere die Arbeitsmappe
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Gibt das [`Cell`](../../cell/)‑Element mit dem angegebenen Zellenamen zurück.

```csharp
public Cell this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellenname, einschließlich seines Spaltenbuchstabens und seiner Zeilennummer, zum Beispiel A5. |

### Rückgabewert

Ein [`Cell`](../../cell/)‑Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greift auf die Zellen-Sammlung zu
            Cells cells = worksheet.Cells;
            
            // Werte mit der Item‑Eigenschaft setzen
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Werte in einem Bereich mit der Item‑Eigenschaft setzen
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Zugriff auf und Modifikation von Zellen‑Eigenschaften mit Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


