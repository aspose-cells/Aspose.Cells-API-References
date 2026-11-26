---
title: "AutoFilter.MatchNonBlanks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Coincidir todas las celdas no vacías en la lista"
type: docs
url: /es/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Coincide con todas las celdas que no están en blanco de la lista.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo con algunas celdas en blanco
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // Aplicar auto filtro para mostrar solo celdas no vacías en la columna A (índice 0)
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Guarda el libro de trabajo
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


