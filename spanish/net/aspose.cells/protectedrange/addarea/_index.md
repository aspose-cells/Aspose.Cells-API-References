---
title: "ProtectedRange.AddArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ProtectedRange. Agrega un área referida a este"
type: docs
url: /es/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Agrega un área referida a este

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio. |
| startColumn | Int32 | La columna de inicio. |
| endRow | Int32 | La fila final. |
| endColumn | Int32 | La columna final. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar devuelve el índice del nuevo ProtectedRange en la colección
            int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];

            try
            {
                protectedRange.AddArea(2, 2, 5, 5);
                Console.WriteLine("Added new area to protected range.");

                CellArea[] areas = protectedRange.GetAreas();
                Console.WriteLine($"Total protected areas: {areas.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            worksheet.Protect(ProtectionType.All, "password123", null);
            workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


