---
title: "Cells.ImportObjectArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa una matriz de datos en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Importa una matriz de datos en una hoja de cálculo.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | Object[] | Matriz de datos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare una matriz de objetos con datos de ejemplo
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Importe la matriz de objetos en la hoja de cálculo comenzando en la celda B3 (fila 2, columna 1), horizontalmente
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Guardar el libro de trabajo para demostrar la salida
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Importa una matriz de datos en una hoja de cálculo.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objArray | Object[] | Matriz de datos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |
| skip | Int32 | Número de filas o columnas omitidas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepare los datos para los parámetros de ImportObjectArray: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // Llame a ImportObjectArray con los parámetros: (matriz de datos, fila de inicio 0, columna de inicio 0, importación horizontal, omitir 1 columna entre entradas)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Demostrar efecto: los datos se colocarán en las celdas A1, C1, E1, A2, C2, E2, etc. con columnas omitidas
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


