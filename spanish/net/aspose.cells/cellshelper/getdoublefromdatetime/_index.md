---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de CellsHelper. Convierte la fecha y hora a un valor double"
type: docs
url: /es/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Convierte la fecha y hora a un valor double.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTime | DateTime | La fecha y hora. |
| date1904 | Booleano | Sistema de fecha 1904. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Crear una instancia de libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la fecha y hora actuales
            DateTime now = DateTime.Now;
            
            // Convertir DateTime a double usando CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Establecer el valor en la celda A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Dar formato a la celda para que se muestre como fecha
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


