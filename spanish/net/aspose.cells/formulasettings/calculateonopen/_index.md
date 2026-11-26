---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaSettings. Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo"
type: docs
url: /es/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Observaciones

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como MS Excel) puedan actuar en consecuencia al cargar el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar el valor que se haya establecido para esta propiedad.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer una fórmula en la celda A1 que haga referencia a B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Establecer un valor en la celda B1
            worksheet.Cells["B1"].PutValue(10);
            
            // Desactivar el cálculo automático de fórmulas al abrir
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Reabrir el libro de trabajo guardado
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Verificar que la fórmula no se haya calculado al abrir
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Calcular fórmulas manualmente
            reopenedWorkbook.CalculateFormula();
            
            // Verificar que la fórmula se haya calculado
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Ver también

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


