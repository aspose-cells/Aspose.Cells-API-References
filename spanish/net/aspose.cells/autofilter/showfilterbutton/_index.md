---
title: "AutoFilter.ShowFilterButton"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFilter. Indica si el botón AutoFilter para esta columna es visible"
type: docs
url: /es/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Indica si el botón AutoFilter para esta columna es visible.

```csharp
public bool ShowFilterButton { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un objeto de lista o tabla
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Habilitar autofiltro y mostrar botones de filtro
            table.AutoFilter.ShowFilterButton = true;

            // Guarda el libro de trabajo
            workbook.Save("output_with_filter_buttons.xlsx");

            // Ocultar botones de filtro
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


