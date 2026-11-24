---
title: "FormatConditionCollection.AddArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Fügt einen bedingt formatierten Zellbereich hinzu"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Fügt einen bedingt formatierten Zellbereich hinzu.

```csharp
public int AddArea(CellArea cellArea)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | Bedingt formatierter Zellbereich. |

### Rückgabewert

Index des bedingt formatierten Zellbereichs.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Formatbedingung erstellen
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Erstelle Zellbereiche und füge sie zur Format-Sammlung hinzu
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


