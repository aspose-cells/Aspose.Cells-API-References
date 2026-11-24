---
title: "Cells.DeleteRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht eine Zeile"
type: docs
url: /de/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Löscht eine Zeile.

```csharp
public void DeleteRow(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Index der zu löschenden Zeile. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Setze eine gemeinsam genutzte Formel in Zeile 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Lösche Zeile 9 (die die Zeilen nach oben verschiebt)
            cells.DeleteRow(9);

            // Überprüfe, dass die Formel nach dem Löschen der Zeile angepasst wurde
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Lösche Zeilen 60-61 (was die Zeilen nach oben verschiebt)
            cells.DeleteRows(59, 2);

            // Überprüfe, ob die Formel nach dem Löschen der Zeilen angepasst wurde
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRow(int, bool) {#deleterow_1}

Löscht eine Zeile.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Index der zu löschenden Zeile. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


