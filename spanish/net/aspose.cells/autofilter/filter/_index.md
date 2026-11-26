---
title: "AutoFilter.Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Filtra una lista con criterios especificados"
type: docs
url: /es/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filtra una lista con criterios especificados.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterio | String | El criterio especificado (una cadena; por ejemplo, "101"). |

### Observaciones

Aspose.Cells eliminará todas las demás configuraciones de filtro en este campo como MS Excel 97-2003.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Aplicar auto filtro usando los parámetros correctos de SetRange
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Guardar el resultado
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


