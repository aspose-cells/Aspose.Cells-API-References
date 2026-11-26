---
title: "CellsHelper.SignificantDigits"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene y establece el número de dígitos significativos. El valor predeterminado es 17"
type: docs
url: /es/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Obtiene y establece el número de dígitos significativos. El valor predeterminado es 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Observaciones

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use [`SignificantDigitsType`](../significantdigitstype/). Esta propiedad será eliminada 12 meses después a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Establecer dígitos significativos
            CellsHelper.SignificantDigits = 15;
            
            // Demostrar el uso de la propiedad
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Crear un libro de trabajo para demostrar los dígitos significativos en los cálculos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valores que serán afectados por los dígitos significativos
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Calcular fórmulas con los dígitos significativos establecidos
            workbook.CalculateFormula();
            
            // Genere la salida de los resultados
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


