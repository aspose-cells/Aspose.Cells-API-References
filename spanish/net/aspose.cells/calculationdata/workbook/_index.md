---
title: "CalculationData.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene el objeto Workbook donde se encuentra la función"
type: docs
url: /es/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Obtiene el objeto Workbook donde está la función.

```csharp
public Workbook Workbook { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra y fórmula
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Crear opciones de cálculo y registrar el motor de cálculo personalizado
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Activar el cálculo con opciones para demostrar el uso de la propiedad Workbook
            workbook.CalculateFormula(options);

            // Mostrar el resultado del cálculo
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Guardar el resultado
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Acceder a la propiedad Workbook desde CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Demostrar el uso de workbook para manipular datos
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Establecer el resultado calculado
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


