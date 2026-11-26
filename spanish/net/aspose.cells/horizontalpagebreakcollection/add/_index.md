---
title: "HorizontalPageBreakCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HorizontalPageBreakCollection. Agrega un salto de página horizontal a la colección"
type: docs
url: /es/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Agrega un salto de página horizontal a la colección.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila, basado en cero. |
| startColumn | Int32 | Índice de columna inicial, basado en cero. |
| endColumn | Int32 | Índice de columna final, basado en cero. |

### Valor de retorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Observaciones

Este método se usa para agregar un salto de página horizontal dentro de un área de impresión.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Demostrar el método Add con parámetros (Int32, Int32, Int32)
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Agrega un salto de página horizontal a la colección.

```csharp
public int Add(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda, basado en cero. |

### Valor de retorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar saltos de página horizontales usando el parámetro Int32
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Agrega un salto de página horizontal a la colección.

```csharp
public int Add(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda, basado en cero. |
| columna | Int32 | Índice de columna de la celda, basado en cero. |

### Valor de retorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para crear varias filas
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Agregar saltos de página horizontales en filas específicas
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Guarda el libro de trabajo
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Agrega un salto de página horizontal a la colección.

```csharp
public int Add(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |

### Valor de retorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Observaciones

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar salto de página horizontal en la fila 4 (D5 es la fila 4 en índice basado en cero)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


