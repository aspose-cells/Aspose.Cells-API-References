---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingValue‑egenskap. Hämta eller ange flaggan för Större än eller lika med. Används endast för ikonsätt och avgör om detta tröskelvärde använder operatorn större än eller lika med. false indikerar att större än används istället för större än eller lika med. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Hämta eller ange flaggan Greater Than Or Equal. Använd endast för ikonuppsättningar, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'greater than' används istället för 'greater than or equal to'. Standardvärdet är true.

```csharp
public bool IsGTE { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Lägg till exempeldata
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Lägg till villkorsstyrd formatering
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Skapa färgskalaformat
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Konfigurera 2‑färgs skala
            fc.ColorScale.Is3ColorScale = false;
            
            // Ställ in maxvärdeformat (demonstrerar IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Ställ in minvärdeformat
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


