---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NumbersLoadOptions. Obtiene y establece el tipo de carga de múltiples tablas en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Obtiene y establece el tipo de carga de múltiples tablas en una hoja de cálculo.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Crear una instancia de NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Demostrar el uso de la propiedad LoadTableType
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Otras propiedades mínimas requeridas
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Cargar un archivo Numbers con las opciones de carga especificadas
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Guardar el libro de trabajo en formato XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


