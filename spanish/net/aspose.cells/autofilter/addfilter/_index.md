---
title: "AutoFilter.AddFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Añade un filtro para una columna de filtro"
type: docs
url: /es/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Añade un filtro para una columna de filtro.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterio | String | El criterio especificado (una cadena; por ejemplo, "101"). Sólo puede ser nulo o ser uno de los valores de celda en esta columna. |

### Observaciones

MS Excel 2007 admite selección múltiple en una columna de filtro.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Crear rango de autofiltro
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Obtener el filtro automático
            AutoFilter filter = worksheet.AutoFilter;
            
            // Añadir filtros para valores que comiencen con 'A' y 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Actualizar el filtro
            filter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


