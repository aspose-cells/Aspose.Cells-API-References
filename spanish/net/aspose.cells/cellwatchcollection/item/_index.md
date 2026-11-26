---
title: "CellWatchCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellWatchCollection. Obtiene y establece CellWatch por índice"
type: docs
url: /es/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Obtiene y establece [`CellWatch`](../../cellwatch/) por índice.

```csharp
public CellWatch this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Demostrar el uso de la propiedad Item
            CellWatch cellWatch = cellWatches[watchIndex];
            
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A1";
            
            Console.WriteLine("\nModified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            workbook.Save("CellWatchCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Obtiene y establece [`CellWatch`](../../cellwatch/) por el nombre de la celda.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | El nombre de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agrega un cell watch a la colección
                int watchIndex = worksheet.CellWatches.Add("A1");

                // Acceder a la CellWatchCollection
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // Demuestre el acceso a la propiedad Item usando el indexador
                CellWatch cellWatch = cellWatches[watchIndex];

                // Mostrar las propiedades del elemento CellWatch
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Guarda el libro de trabajo
                workbook.Save("CellWatchItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


