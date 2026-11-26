---
title: "LoadOptions.CheckDataValid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Verifique si los datos son válidos en el archivo de plantilla"
type: docs
url: /es/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Verificar si los datos son válidos en el archivo de plantilla.

```csharp
public bool CheckDataValid { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // Cree opciones de carga con CheckDataValid establecido en false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Cargue el libro de trabajo con estas opciones
            Workbook workbook = new Workbook("example.xlsx", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue alguna validación de datos para la demostración
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Establecer el rango de validación
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


