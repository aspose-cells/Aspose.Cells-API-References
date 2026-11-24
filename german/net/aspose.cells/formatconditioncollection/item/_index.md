---
title: "FormatConditionCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Eigenschaft. Gibt die Formatierungsbedingung nach Index zurück"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Gibt die Formatierungsbedingung nach Index zurück.

```csharp
public FormatCondition this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index der zurückzugebenden Formatierungsbedingung. |

### Rückgabewert

die Formatierungsbedingung

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge eine Formatierungsbedingungssammlung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Füge eine Formatierungsbedingung hinzu
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Greife auf die erste Formatierungsbedingung über die Item-Eigenschaft zu
            FormatCondition condition = fcc[0];
            
            // Zeige die Formeln an
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Ändere die Formeln über die Item-Eigenschaft
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Zeige die geänderten Formeln an
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


