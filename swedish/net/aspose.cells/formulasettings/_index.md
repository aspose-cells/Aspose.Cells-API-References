---
title: "Klass FormulaSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormulaSettings-klass. Inställningar för formler och beräkning"
type: docs
url: /sv/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Inställningar för formler och beräkning.

```csharp
public class FormulaSettings
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Anger om arbetsboken ska omberäknas innan dokumentet sparas, när man är i manuellt beräkningsläge. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Hämtar eller anger läget för arbetsboksberäkning i MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Anger om beräkningskedjan för formler ska aktiveras. Standard är falskt. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Anger om alla formler beräknas varje gång en beräkning utlöses. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | Den maximala förändringen för att lösa en cirkulär referens. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Det maximala antalet iterationer för att lösa en cirkulär referens. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Anger om precisionen för beräknat resultat ska sättas som de visas under beräkning av formler. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbokens formelinställningar
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Ställa in egenskaper
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Spara arbetsboken
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


