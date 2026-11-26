---
title: "Validation.InCellDropDown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables"
type: docs
url: /es/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables.

```csharp
public bool InCellDropDown { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una validación para la celda A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Establecer el tipo de validación a lista con valores
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Habilitar lista desplegable en la celda
            validation.InCellDropDown = true;

            // Crear otra validación para la celda B1 sin lista desplegable
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Guarda el libro de trabajo
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


