---
title: "HorizontalPageBreakCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HorizontalPageBreakCollection. Obtiene el elemento HorizontalPageBreak en el índice especificado"
type: docs
url: /es/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Obtiene el elemento [`HorizontalPageBreak`](../../horizontalpagebreak/) en el índice especificado.

```csharp
public HorizontalPageBreak this[int index] { get; }
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
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue saltos de página horizontales
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Acceder a los saltos de página usando la propiedad Item
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modificar celdas que afectan los saltos de página
            worksheet.Cells.DeleteRows(0, 2);
            
            // Verificar que el salto de página fue ajustado
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Ver también

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Obtiene el elemento [`HorizontalPageBreak`](../../horizontalpagebreak/) con el nombre de celda especificado.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
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
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un par de saltos de página horizontales usando diferentes sobrecargas
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Acceso mediante índice entero (Item[int]) -----
                // La propiedad Item es el indexador, por lo que usamos la sintaxis []
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Acceso mediante clave de cadena (Item[string]) -----
                // Recuperar el salto de página que se añadió con el nombre de celda "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Guardar el libro de trabajo para verificar que los saltos de página se persisten
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


