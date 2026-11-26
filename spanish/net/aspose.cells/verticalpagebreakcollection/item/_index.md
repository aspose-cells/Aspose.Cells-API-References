---
title: "VerticalPageBreakCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VerticalPageBreakCollection. Obtiene el elemento VerticalPageBreak en el índice especificado"
type: docs
url: /es/net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Obtiene el elemento [`VerticalPageBreak`](../../verticalpagebreak/) en el índice especificado.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar saltos de página verticales
            worksheet.VerticalPageBreaks.Add(5);
            worksheet.VerticalPageBreaks.Add(10);
            worksheet.VerticalPageBreaks.Add(15);

            // Acceder y mostrar los saltos de página usando la propiedad Item
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < vpagebreaks.Count; i++)
            {
                Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
            }

            // Eliminar y volver a agregar para modificar un salto de página ya que Column es de solo lectura
            int column = vpagebreaks[1].Column;
            vpagebreaks.RemoveAt(1);
            vpagebreaks.Add(12);
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
        }
    }
}
```

### Ver también

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Obtiene el elemento [`VerticalPageBreak`](../../verticalpagebreak/) con el nombre de celda especificado.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | Nombre de la celda. |

### Valor de retorno

El elemento con el nombre de celda especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos saltos de página verticales
            worksheet.VerticalPageBreaks.Add(3);
            worksheet.VerticalPageBreaks.Add(7);

            try
            {
                // Acceder a la VerticalPageBreakCollection
                VerticalPageBreakCollection pageBreaks = worksheet.VerticalPageBreaks;

                // Demostrar el acceso a los elementos usando la propiedad Item (indexador)
                Console.WriteLine("Vertical Page Breaks in the worksheet:");
                for (int i = 0; i < pageBreaks.Count; i++)
                {
                    VerticalPageBreak vpb = pageBreaks[i];
                    Console.WriteLine($"Break {i + 1}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
                }

                // Guarda el libro de trabajo
                workbook.Save("VerticalPageBreakItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


