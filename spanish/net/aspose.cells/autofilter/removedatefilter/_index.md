---
title: "AutoFilter.RemoveDateFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Elimina un filtro de fecha"
type: docs
url: /es/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Elimina un filtro de fecha.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| dateTimeGroupingType | DateTimeGroupingType | El tipo de agrupación |
| año | Int32 | El año. |
| mes | Int32 | El mes. |
| día | Int32 | El día. |
| hora | Int32 | La hora. |
| minuto | Int32 | El minuto. |
| segundo | Int32 | El segundo. |

### Observaciones

Si DateTimeGroupingType es Year, solo el parámetro year tiene efecto. Si DateTiemGroupingType es Month, solo los parámetros year y month tienen efecto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de muestra con fechas
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Aplicar filtro automático
            sheet.AutoFilter.Range = "A1:A4";
            
            // Agregar filtro de fecha para el día 7
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verificar que el filtro se haya aplicado
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Eliminar el filtro de fecha
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verificar que el filtro se haya eliminado
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### Ver también

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


