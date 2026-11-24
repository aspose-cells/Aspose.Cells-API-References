---
title: "FormatConditionCollection.RemoveArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Entfernt den bedingt formatierten Zellbereich nach Index"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Entfernt den bedingt formatierten Zellbereich nach Index.

```csharp
public void RemoveArea(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des bedingt formatierten Zellbereichs, der entfernt werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Bereiche zum Formatieren hinzufügen
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Eine Bedingung hinzufügen
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Anzahl der Anfangsbereiche anzeigen (wir wissen, dass wir 2 Bereiche hinzugefügt haben)
            Console.WriteLine("Areas before removal: 2");

            // Den zweiten Bereich entfernen (Index 1)
            formatConditionCollection.RemoveArea(1);

            // Anzahl der Bereiche nach dem Entfernen anzeigen (wir wissen, dass wir 1 Bereich entfernt haben)
            Console.WriteLine("Areas after removal: 1");

            // Speichere die Arbeitsmappe
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Entferne die bedingte Formatierung im Bereich.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile des Bereichs. |
| startColumn | Int32 | Die Startspalte des Bereichs. |
| totalRows | Int32 | Die Anzahl der Zeilen des Bereichs. |
| totalColumns | Int32 | Die Anzahl der Spalten des Bereichs. |

### Rückgabewert

Gibt TRUE zurück, diese FormatCondtionCollection sollte entfernt werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Anfangsbereich hinzufügen
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Bedingung hinzufügen
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Demonstriere RemoveArea mit Int32-Parametern
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Neuen Bereich hinzufügen
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Siehe auch

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


