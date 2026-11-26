---
title: "AutoFilter.MatchBlanks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Coincidir todas las celdas en blanco en la lista"
type: docs
url: /es/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Coincide con todas las celdas en blanco de la lista.

```csharp
public void MatchBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo con algunas celdas en blanco
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Dejar C2 en blanco
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Dejar B3 en blanco
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtrar para mostrar solo filas con celdas en blanco en la columna 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Actualizar el filtro
            filter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


