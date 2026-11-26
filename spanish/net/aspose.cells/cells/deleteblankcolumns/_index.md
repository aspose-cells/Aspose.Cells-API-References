---
title: "Cells.DeleteBlankColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina todas las columnas en blanco que no contienen datos"
type: docs
url: /es/net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Elimina todas las columnas en blanco que no contengan ningún dato.

```csharp
public void DeleteBlankColumns()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de prueba con columnas en blanco
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
            worksheet.Cells["A2"].PutValue("Data A");
            worksheet.Cells["C2"].PutValue("Data C");
            
            // Eliminar columnas en blanco
            worksheet.Cells.DeleteBlankColumns();
            
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

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Elimina todas las columnas en blanco que no contengan ningún dato.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | DeleteOptions | Las opciones de eliminación del rango. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos con columnas en blanco
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["C2"].PutValue(3);

            Console.WriteLine("Before deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)

            // Configurar opciones de eliminación
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;

            // Eliminar columnas en blanco
            worksheet.Cells.DeleteBlankColumns(options);

            Console.WriteLine("After deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)

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


