---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si se deben conservar esos espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indica si se deben conservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Observaciones

En general, esos espacios y saltos de línea son solo con fines visuales; conservarlos o no no afecta el resultado calculado. Por consideraciones de rendimiento, si no hay un requisito especial, es mejor no conservarlos al procesar fórmulas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer fórmula con espacios de relleno
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Comportamiento predeterminado (PreservePaddingSpaces es true)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Cambiar la configuración para eliminar los espacios de relleno
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Guarda el libro de trabajo
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


