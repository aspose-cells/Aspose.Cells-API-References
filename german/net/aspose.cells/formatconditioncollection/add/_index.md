---
title: "FormatConditionCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. Verweise auf andere Tabellenblätter sind in den Formeln der bedingten Formatierung nicht zulässig."
type: docs
url: /de/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. Verweise auf andere Tabellenblätter sind in den Formeln der bedingten Formatierung nicht zulässig.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | Bedingt formatierter Zellbereich. |
| Typ | FormatConditionType | Typ der bedingten Formatierung. Es könnte einer der Mitglieder von FormatConditionType sein. |
| operatorType | OperatorType | Vergleichsoperator. Es könnte einer der Mitglieder von OperatorType sein. |
| formula1 | String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| formula2 | String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist |

### Rückgabewert

[0]:Formatting condition object index;[1] Effected cell rang index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Beispieldaten befüllen
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Demonstriere die Add-Methode mit angegebenen Parametern
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Formatierung anwenden
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Speichere die Arbeitsmappe, um das Ergebnis zu demonstrieren
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


