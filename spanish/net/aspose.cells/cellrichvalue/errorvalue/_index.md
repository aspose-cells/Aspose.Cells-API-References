---
title: "CellRichValue.ErrorValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellRichValue. Obtiene el tipo de valor de error de la celda"
type: docs
url: /es/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Obtiene el tipo de valor de error de la celda.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un error de desbordamiento en la celda A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Calcular fórmulas para generar el error de desbordamiento
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Error de desbordamiento esperado
            }
            
            // Obtener el valor enriquecido de la celda A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Verificar y mostrar el tipo de error
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


