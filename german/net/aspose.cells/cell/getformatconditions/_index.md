---
title: "Cell.GetFormatConditions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt Formatbedingungen zurück, die für diese Zelle gelten"
type: docs
url: /de/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Liefert Formatbedingungen, die für diese Zelle gelten.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Rückgabewert

Gibt das [`FormatConditionCollection`](../../formatconditioncollection/) Objekt zurück

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellsammlung abrufen
            Cells cells = worksheet.Cells;
            
            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Formatbedingung zu Zelle A1 hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Formatbedingungen für Zelle A1 abrufen
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Gibt die Anzahl der Formatbedingungen aus
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


