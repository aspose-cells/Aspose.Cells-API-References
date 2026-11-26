---
title: "ProtectedRange.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRange. Obtiene el título del rango. Esto se usa como descriptor, no como una definición de rango con nombre"
type: docs
url: /es/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Obtiene el título del rango. Se usa como descriptor, no como una definición de rango con nombre.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear colección de rangos protegidos
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Agregar un rango protegido con el nombre "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Acceder y mostrar la propiedad Name
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Agregar otro rango con nombre
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


