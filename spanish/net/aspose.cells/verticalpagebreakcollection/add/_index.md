---
title: "VerticalPageBreakCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VerticalPageBreakCollection. Agrega un salto de página vertical a la colección"
type: docs
url: /es/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Agrega un salto de página vertical a la colección.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila de inicio, basado en cero. |
| endRow | Int32 | Índice de fila final, basado en cero. |
| columna | Int32 | Índice de columna, basado en cero. |

### Valor de retorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Observaciones

Este método se usa para agregar un salto de página vertical dentro de un área de impresión.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // Demostrar Add con parámetros (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Ejemplos adicionales para contexto
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Agrega un salto de página vertical a la colección.

```csharp
public int Add(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna de la celda, basado en cero. |

### Valor de retorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Demostrar el método Add con parámetro Int32
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Imprimir los detalles del salto de página agregado
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Agrega un salto de página vertical a la colección.

```csharp
public int Add(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda, basado en cero. |
| columna | Int32 | Índice de columna de la celda, basado en cero. |

### Valor de retorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de saltos de página verticales
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Agregar saltos de página verticales en diferentes posiciones de columna
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Agregar datos de muestra para visualizar los saltos de página
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Guarda el libro de trabajo
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Agrega un salto de página vertical a la colección.

```csharp
public int Add(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |

### Valor de retorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Ver también

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


