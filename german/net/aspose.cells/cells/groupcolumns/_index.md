---
title: "Cells.GroupColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gruppiert Spalten"
type: docs
url: /de/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Gruppiert Spalten.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der erste Spaltenindex, der gruppiert werden soll. |
| lastIndex | Int32 | Der letzte Spaltenindex, der gruppiert werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spalten von Index 0 bis 255 gruppieren
            cells.GroupColumns(0, 255);

            // Speichere die Arbeitsmappe
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Gruppiert Spalten.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der erste Spaltenindex, der gruppiert werden soll. |
| lastIndex | Int32 | Der letzte Spaltenindex, der gruppiert werden soll. |
| isHidden | Boolean | Gibt an, ob die gruppierten Spalten ausgeblendet sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spalten 5 bis 7 (3 Spalten) gruppieren und ausblenden
            cells.GroupColumns(5, 7, true);

            // Speichere die Arbeitsmappe
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


