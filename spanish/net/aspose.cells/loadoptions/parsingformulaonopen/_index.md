---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se analiza la fórmula al leer el archivo"
type: docs
url: /es/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Indica si se analiza la fórmula al leer el archivo.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Observaciones

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm y Xlsm porque las fórmulas en los archivos se almacenan como una fórmula de cadena.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Crear opciones de carga
            LoadOptions loadOptions = new LoadOptions();
            
            // Establecer ParsingFormulaOnOpen en false para omitir el análisis de fórmulas durante la carga
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Cargar el libro de trabajo con las opciones especificadas
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Acceder a la hoja de cálculo y demostrar que el análisis de fórmulas se omitió
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


