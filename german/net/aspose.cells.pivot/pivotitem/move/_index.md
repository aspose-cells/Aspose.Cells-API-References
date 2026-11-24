---
title: "PivotItem.Move"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Methode. Verschiebt das Element nach oben oder unten"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Verschiebt das Element nach oben oder unten

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Versatz | Int32 | Die Anzahl der Verschiebungen nach oben oder unten. Verschiebe das Element nach oben, wenn dieser Wert kleiner als null ist; verschiebe das Element nach unten, wenn er größer als null ist. |
| isSameParent | Boolean | Angabe, ob die Verschiebeoperation im selben übergeordneten Knoten stattfindet oder nicht |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen PivotTable.MoveItem(PivotFieldType, string[],bool,int) oder die PivotItem.Move(int)-Methode. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispieldaten für Pivot‑Tabelle erstellen
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Abrufen von Pivot-Elementen und Demonstration der Move-Methode
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Verschiebe das erste Element zu Position 1 (zweite Position) mit Unterelementen
            items[0].Move(1, true);
            
            // Speichere die Arbeitsmappe
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Verschiebt das Element nach oben oder unten im Pivot-Feld

```csharp
public void Move(int offset)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Versatz | Int32 | Die Anzahl der Verschiebungen nach oben oder unten. Verschiebe das Element nach oben, wenn dieser Wert kleiner als null ist; verschiebe das Element nach unten, wenn er größer als null ist. |

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


