---
title: "FilterColumnCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumnCollection. Obtiene el objeto FilterColumn en el campo especial"
type: docs
url: /es/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Obtiene el objeto [`FilterColumn`](../../filtercolumn/) en el campo especial.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fieldIndex | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |

### Valor de retorno

Devuelve el objeto [`FilterColumn`](../../filtercolumn/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Aplicar filtro automático
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Acceda al filtro usando la propiedad Item
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Mostrar propiedades del filtro
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Modificar filtro
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Guarda el libro de trabajo
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


