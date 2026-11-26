---
title: "Enumeración CalcModeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.CalcModeType. Representa el tipo de modo de cálculo de fórmulas"
type: docs
url: /es/net/aspose.cells/calcmodetype/
---
## CalcModeType enumeration

Representa el tipo de modo de cálculo de fórmulas.

```csharp
public enum CalcModeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |

### Observaciones

Solo configuraciones para MS Excel.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalcModeTypeDemo
    {
        public static void CalcModeTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la prueba
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            worksheet.Cells["A4"].Formula = "=A1+B1+C1";
            worksheet.Cells["B4"].Formula = "=SUM(B1:B3)";

            // Acceda a la configuración de fórmulas del libro de trabajo
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Establezca el modo de cálculo a Manual
            formulaSettings.CalculationMode = CalcModeType.Manual;

            // Establezca otras configuraciones de fórmulas
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Guarda el libro de trabajo
            workbook.Save("CalcModeTypeExample.xlsx");
            workbook.Save("CalcModeTypeExample.pdf");

        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


