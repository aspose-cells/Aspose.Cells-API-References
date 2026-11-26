---
title: "Row.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Obtiene el enumerador de celdas"
type: docs
url: /es/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Obtiene el enumerador de celdas

```csharp
public IEnumerator GetEnumerator()
```

### Valor de retorno

El enumerador de celdas que recorrerá todas las celdas existentes en esta fila.

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Obtener enumerador para la primera fila (fila de encabezado)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Obtiene un enumerador que recorre las celdas a través de esta fila.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| invertido | Booleano | si enumerar celdas en orden inverso |
| sync | Booleano | si el enumerador devuelto debe comprobar la modificación de las celdas en esta fila y mantenerse sincronizado con ella. |

### Valor de retorno

El enumerador de celdas que recorrerá todas las celdas existentes en esta fila.

### Observaciones

Si la fila se modifica (por operaciones que pueden provocar que se instancie una nueva Cell o que se elimine una Cell existente) durante el recorrido con el enumerador, se debe usar un enumerador sincronizado en lugar de un enumerador normal para que el recorrido pueda continuar desde la posición justo después de la que fue recorrida por el último MoveNext(). Sin embargo, junto con la ventaja de que no se omita ni se recorra repetidamente ningún elemento, la desventaja del enumerador sincronizado es que el rendimiento se degradará un poco en comparación con el enumerador normal.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas en la primera fila
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Llamar a GetEnumerator con reversed=false y sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Llamar a GetEnumerator con reversed=true y sync=false para demostrar la iteración inversa
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


