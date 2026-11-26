---
title: "AutoFilter.RemoveFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Elimina un filtro para una columna de filtro"
type: docs
url: /es/net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

Elimina un filtro para una columna de filtro.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterio | String | El criterio especificado (una cadena; por ejemplo, "101"). Sólo puede ser nulo o ser uno de los valores de celda en esta columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de muestra para la demostración
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // Establecer rango de autofiltro (encabezados + 3 filas de datos)
            worksheet.AutoFilter.SetRange(0, 0, 2);

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // Aplicar filtro en la columna Category (fieldIndex 1) para "Electronics"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows
                
                // Eliminar el filtro específico de la columna Category
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

Elimina el filtro específico.

```csharp
public void RemoveFilter(int fieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El índice del filtro específico |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveFilterWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Agregar un filtro
            filter.AddFilter(0, "Apple");
            filter.Refresh();
            
            Console.WriteLine("After adding filter - Visible rows:");
            PrintVisibleRows(worksheet);
            
            // Eliminar el filtro
            filter.RemoveFilter(0);
            filter.Refresh();
            
            Console.WriteLine("\nAfter removing filter - Visible rows:");
            PrintVisibleRows(worksheet);
        }
        
        private static void PrintVisibleRows(Worksheet worksheet)
        {
            for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
            {
                if (!worksheet.Cells.Rows[i].IsHidden)
                {
                    Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
                }
            }
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


