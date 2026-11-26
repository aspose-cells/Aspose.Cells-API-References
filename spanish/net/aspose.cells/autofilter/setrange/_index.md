---
title: "AutoFilter.SetRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Establece el rango al que se aplica el AutoFilter especificado"
type: docs
url: /es/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Establece el rango al que se aplica el AutoFilter especificado.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| startColumn | Int32 | Índice de columna inicial. |
| endColumn | Int32 | Índice de columna final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Establecer rango de autofiltro (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Aplicar filtro
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Actualizar filtro
            sheet.AutoFilter.Refresh();

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


