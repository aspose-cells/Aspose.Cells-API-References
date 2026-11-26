---
title: "FormulaSettings.CalculateOnSave"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si se debe recalcular el libro de trabajo antes de guardar el documento cuando está en modo de cálculo manual"
type: docs
url: /es/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual.

```csharp
public bool CalculateOnSave { get; set; }
```

### Observaciones

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos automáticamente ninguna fórmula en el libro de trabajo, sin importar el valor que se haya establecido para esta propiedad.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la hoja de cálculo y agregar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Desactivar CalculateOnSave (el valor predeterminado es false)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Guardar sin calcular fórmulas
            workbook.Save("output_without_calculation.xlsx");

            // Activar CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Guardar con cálculo de fórmulas
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


