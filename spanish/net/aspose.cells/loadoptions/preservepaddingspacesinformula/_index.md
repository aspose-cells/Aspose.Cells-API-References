---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Observaciones

Después de cargar el libro de trabajo desde el archivo de plantilla con esta opción, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) se establecerá al mismo valor que esta propiedad.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Habilitar la conservación de espacios de relleno en fórmulas
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Acceder a la primera hoja de cálculo y establecer una fórmula con espacios de relleno
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Guardar y volver a cargar el libro de trabajo con la opción PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Verificar que la fórmula conserva los espacios después de recargar
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


