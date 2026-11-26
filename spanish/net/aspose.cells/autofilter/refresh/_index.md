---
title: "AutoFilter.Refresh"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Refresca los auto filters para ocultar o mostrar las filas"
type: docs
url: /es/net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Actualiza los autofiltros para ocultar o mostrar las filas.

```csharp
public int[] Refresh()
```

### Valor de retorno

Devuelve los índices de todas las filas ocultas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["B6"].PutValue("Header1");
            worksheet.Cells["C6"].PutValue("Header2");
            worksheet.Cells["D6"].PutValue("Header3");
            worksheet.Cells["E6"].PutValue("Values");
            
            for (int i = 7; i <= 15; i++)
            {
                worksheet.Cells["B" + i].PutValue("Item " + (i-6));
                worksheet.Cells["E" + i].PutValue((i-6) * 100);
            }

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "B6:E6";
            
            // Filtrar valores mayores que 500
            worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
            
            // Cambiar el filtro para mostrar valores iguales a 500 o mayores que 700
            worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Obtiene los índices de todas las filas ocultas.

```csharp
public int[] Refresh(bool hideRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hideRows | Booleano | Si es verdadero, ocultar las filas filtradas. |

### Valor de retorno

Devuelve todos los índices de filas ocultas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(1);
            worksheet.Cells["A5"].PutValue(3);
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
            
            // Actualizar el filtro y obtener filas ocultas
            int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("Hidden rows after filter:");
            if (hiddenRows != null)
            {
                foreach (int row in hiddenRows)
                {
                    Console.WriteLine(row);
                }
            }
            
            // Mostrar todos los datos y actualizar nuevamente
            worksheet.AutoFilter.ShowAll();
            hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("\nHidden rows after showing all:");
            if (hiddenRows == null)
            {
                Console.WriteLine("No hidden rows");
            }
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


