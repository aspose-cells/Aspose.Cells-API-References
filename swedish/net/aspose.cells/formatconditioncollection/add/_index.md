---
title: "FormatConditionCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection-metod. Lägger till ett formateringsvillkor och påverkade cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorsformat. Referenser till andra blad är inte tillåtna i formlerna för villkorsformatering."
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Lägger till ett formateringsvillkor och påverkad cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorliga format. Referenser till andra blad är inte tillåtna i formlerna för villkorlig formatering.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Villkorsformaterat cellområde. |
| typ | FormatConditionType | Typ av villkorsformatering. Det kan vara en av medlemmarna i FormatConditionType. |
| operatorType | OperatorType | Jämförelseoperator. Det kan vara en av medlemmarna i OperatorType. |
| formula1 | String | Värdet eller uttrycket som är kopplat till villkorsformatering. |
| formula2 | String | Värdet eller uttrycket som är kopplat till villkorsformatering |

### Returvärde

[0]:Formatting condition object index;[1] Effected cell rang index.

### Exempel

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
            
            // Fyll i exempeldata
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Demonstrera Add-metoden med angivna parametrar
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Applicera formatering
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Spara arbetsboken för att demonstrera resultatet
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


