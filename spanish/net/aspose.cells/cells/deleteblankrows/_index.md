---
title: "Cells.DeleteBlankRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina todas las filas en blanco que no contienen datos ni otros objetos"
type: docs
url: /es/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Elimina todas las filas en blanco que no contengan ningún dato u otro objeto.

```csharp
public void DeleteBlankRows()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar algunos datos con filas en blanco
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Eliminar filas en blanco
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Elimina todas las filas en blanco que no contengan ningún dato o algunos objetos especiales como comentarios visibles, tabla dinámica.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | DeleteOptions | Las opciones de eliminación del rango. |

### Observaciones

Para las filas en blanco que se eliminarán, no solo se requiere que [`IsBlank`](../../row/isblank/) sea verdadero, sino que también no debe haber ningún comentario visible definido para cualquier celda en esas filas, y ninguna tabla dinámica cuyo rango intersecte con ellas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de prueba con filas en blanco
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Crear opciones de eliminación
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Eliminar filas en blanco
            sheet.Cells.DeleteBlankRows(options);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


