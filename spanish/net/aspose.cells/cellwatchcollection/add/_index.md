---
title: "CellWatchCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellWatchCollection. Añade CellWatch con una fila y una columna"
type: docs
url: /es/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Añade [`CellWatch`](../../cellwatch/) con una fila y una columna.

```csharp
public int Add(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

Devuelve la posición de este elemento en la colección.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenga la CellWatchCollection de la hoja de cálculo
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Llame al método Add con los índices de fila y columna (Int32, Int32)
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Verifique el cell watch agregado
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Agrega [`CellWatch`](../../cellwatch/) con el nombre de la celda.

```csharp
public int Add(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | El nombre de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunas observaciones de celda
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Muestra el recuento de cell watches
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


