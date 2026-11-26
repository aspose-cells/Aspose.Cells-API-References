---
title: "AutoFilter.FilterTop10"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Filtra los 10 principales elementos de la lista"
type: docs
url: /es/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filtrar los 10 elementos principales de la lista

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| isTop | Booleano | Indica si el filtro es desde la parte superior o inferior |
| isPercent | Booleano | Indica si los elementos son porcentaje o recuento |
| itemCount | Int32 | El recuento de elementos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra (5 filas x 3 columnas con valores numéricos)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Establecer rango de autofiltro
            worksheet.AutoFilter.Range = "A1:A6";

            // Aplicar filtro de los 10 principales (mostrando los 2 primeros elementos)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Actualizar el filtro
            worksheet.AutoFilter.Refresh();

            // Guarda el libro de trabajo
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


