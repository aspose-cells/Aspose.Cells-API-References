---
title: "Name.SheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Indica que este nombre pertenece a Workbook o Worksheet. 0  Nombre global, de lo contrario índice a la hoja basado en uno"
type: docs
url: /es/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indica a qué pertenece este nombre: Libro de trabajo o Hoja de cálculo. 0 = Nombre global, de lo contrario índice a la hoja (basado en uno).

```csharp
public int SheetIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crear un rango con nombre en Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Mostrar el índice de hoja del rango con nombre
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Guarda el libro de trabajo
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


