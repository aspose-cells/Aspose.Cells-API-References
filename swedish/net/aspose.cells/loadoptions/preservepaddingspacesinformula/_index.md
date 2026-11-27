---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och sättning av formler. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Anmärkningar

Efter att arbetsboken har laddats från mallfil med detta alternativ, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) kommer att sättas till samma värde som denna egenskap.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Aktivera bevarande av utfyllda mellanslag i formler
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Öppna första kalkylbladet och ange en formel med utfyllda mellanslag
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Spara och ladda om arbetsboken med PreservePaddingSpacesInFormula‑alternativet
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Verifiera att formeln bevarade mellanslag efter omladdning
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


