---
title: "Enumeración LookAtType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.LookAtType. Representa el tipo de búsqueda"
type: docs
url: /es/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Representa el tipo de visualización.

```csharp
public enum LookAtType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Contains | `0` | El valor de la celda contiene el objeto de búsqueda. |
| StartWith | `1` | El valor de la celda comienza con el objeto de búsqueda. |
| EndWith | `2` | El valor de la celda termina con el objeto de búsqueda. |
| EntireContent | `3` | El valor de la celda es igual al objeto de búsqueda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Instanciar el objeto libro de trabajo
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Obtener la colección Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Instanciar el objeto FindOptions
            FindOptions findOptions = new FindOptions();

            // Crear un área Cells
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Establecer el área de celdas para las opciones de búsqueda
            findOptions.SetRange(ca);

            // Establecer propiedades de búsqueda
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Establecer LookAtType a Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Buscar la celda con un valor específico
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


