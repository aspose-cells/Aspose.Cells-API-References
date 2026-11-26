---
title: "Enum LoadNumbersTableType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Numbers.LoadNumbersTableType. Indica el tipo de carga de tablas cuando algunas tablas están en una hoja"
type: docs
url: /es/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Indica el tipo de carga de tablas cuando algunas tablas están en una hoja.

```csharp
public enum LoadNumbersTableType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una nueva hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Establecer la propiedad LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Cargar un archivo Numbers con las opciones de carga especificadas
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


