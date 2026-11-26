---
title: "InsertOptions.UpdateReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad InsertOptions. Indica si las referencias en otras hojas de cálculo se actualizarán"
type: docs
url: /es/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Indica si las referencias en otras hojas de cálculo se actualizarán.

```csharp
public bool UpdateReference { get; set; }
```

### Observaciones

A partir de la versión 26.7 establecemos el valor predeterminado de esta propiedad en true.

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar una segunda hoja de cálculo y establecer fórmulas que hacen referencia a Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Establecer fórmulas en Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Crear opciones de inserción con UpdateReference habilitado
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Rastrear cambios de fórmula
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Insertar filas que actualizarán las referencias en las fórmulas
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Mostrar la cantidad de celdas modificadas
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Mostrar las fórmulas actualizadas
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Ver también

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


