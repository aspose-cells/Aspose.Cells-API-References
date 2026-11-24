---
title: "PivotTable.GetChildren"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die untergeordneten Pivot-Tabellen zurück, die diese PivotTable-Daten als Datenquelle verwenden."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Gibt die untergeordneten Pivot-Tabellen zurück, die diese PivotTable-Daten als Datenquelle verwenden.

```csharp
[Obsolete("Use PivotTable.GetDependentPivotTables() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotTable[] GetChildren()
```

### Rückgabewert

das PivotTable-Array-Objekt

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode PivotTable.GetDependentPivotTables(). Diese Methode wird 12 Monate nach April 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetChildrenDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Haupt-Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
            PivotTable mainPivotTable = pivotTables[index];
            mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Untergeordnete Pivot-Tabelle erstellen
            index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
            PivotTable childPivotTable = pivotTables[index];
            childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Beziehung herstellen, indem Basisfelder geteilt werden
            foreach (PivotField field in mainPivotTable.BaseFields)
            {
                childPivotTable.BaseFields.Add(field);
            }

            // GetChildren()-Methode demonstrieren
            Console.WriteLine("Child Pivot Tables:");
            foreach (PivotTable child in mainPivotTable.GetChildren())
            {
                Console.WriteLine("Child Pivot Table Name: " + child.Name);
                Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


