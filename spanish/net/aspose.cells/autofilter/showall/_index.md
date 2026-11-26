---
title: "AutoFilter.ShowAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Mostrar todas las filas"
type: docs
url: /es/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Desocultar todas las filas.

```csharp
public void ShowAll()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Filtrar para mostrar solo "Apple"
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Mostrar todos los datos de nuevo
            worksheet.AutoFilter.ShowAll();
            
            // Guarda el libro de trabajo
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


