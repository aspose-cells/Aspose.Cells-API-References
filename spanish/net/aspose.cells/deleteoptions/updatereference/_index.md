---
title: "DeleteOptions.UpdateReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteOptions. Indica si se actualizan referencias en otras hojas de cálculo"
type: docs
url: /es/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Indica si actualizar referencias en otras hojas de cálculo.

```csharp
public bool UpdateReference { get; set; }
```

### Observaciones

A partir de la versión 26.7 establecemos el valor predeterminado de esta propiedad en true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y fórmulas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Cree opciones de eliminación con UpdateReference establecido en verdadero
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Elimine la columna A que está referenciada en fórmulas
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


