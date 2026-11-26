---
title: "ProtectedRange.GetAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ProtectedRange. Obtiene todas las áreas referidas"
type: docs
url: /es/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Obtiene todas las áreas referidas.

```csharp
public CellArea[] GetAreas()
```

### Valor de retorno

Devuelve todas las áreas referidas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la colección de rangos protegidos
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Agregar un rango protegido
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Obtener áreas del rango protegido
            CellArea[] areas = protectedRange.GetAreas();
            
            // Mostrar el número de áreas (debe ser 1 para este rango simple)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


