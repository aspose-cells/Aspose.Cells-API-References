---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Entfernt die Formatierungsbedingung nach Index"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Entfernt die Formatierungsbedingung nach Index.

```csharp
public void RemoveCondition(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index der zu entfernenden Formatierungsbedingung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rufe die Sammlung der Formatierungsbedingungen ab
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Füge einige Beispielbedingungen hinzu
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Zeige die anfängliche Anzahl an
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Entferne die erste Bedingung
                formatConditions.RemoveCondition(index1);
                
                // Zeige die aktualisierte Anzahl an.
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


