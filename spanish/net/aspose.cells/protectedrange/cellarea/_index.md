---
title: "ProtectedRange.CellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRange. Obtiene el objeto CellArea que representa el área de celdas a proteger"
type: docs
url: /es/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Obtiene el objeto `CellArea` que representa el área de celdas a proteger.

```csharp
public CellArea CellArea { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear rangos protegidos
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Agregar el primer rango protegido
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Agregar el segundo rango protegido
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Mostrar información de CellArea para ambos rangos
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


