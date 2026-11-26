---
title: "Clase FindOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FindOptions. Representa opciones de búsqueda"
type: docs
url: /es/net/aspose.cells/findoptions/
---
## FindOptions class

Representa opciones de búsqueda.

```csharp
public class FindOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FindOptions](findoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indica si la cadena buscada distingue entre mayúsculas y minúsculas. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si se convierte el valor de la cadena buscada a datos numéricos. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsoleto.**) Indica si la cadena buscada distingue entre mayúsculas y minúsculas. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Indica si el rango buscado está establecido. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Buscar tipo. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Buscar en tipo. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Indica si la clave buscada es una expresión regular. Si es verdadero, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará según las reglas de MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Indica si se busca hacia atrás en las celdas. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Orden de búsqueda. Verdadero: buscar siguiente. Falso: buscar anterior. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Indica si el orden de búsqueda es por filas o por columnas. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | El formato a buscar. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Obtiene y establece el rango buscado. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Establece el rango buscado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Instanciar el objeto libro de trabajo
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Obtener la colección Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Instanciar el objeto FindOptions
            FindOptions findOptions = new FindOptions();

            // Crear un área Cells
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Establecer el área de celdas para las opciones de búsqueda
            findOptions.SetRange(ca);

            // Establecer propiedades de búsqueda
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Buscar la celda con valor 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
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


