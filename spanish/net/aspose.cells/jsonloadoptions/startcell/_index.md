---
title: "JsonLoadOptions.StartCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLoadOptions. Obtiene y establece la celda inicial"
type: docs
url: /es/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Obtiene y establece la celda inicial.

```csharp
public string StartCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Crear opciones de carga JSON con la propiedad StartCell
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Crear un libro de trabajo a partir de un archivo JSON con opciones
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Crear un archivo JSON de ejemplo
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // Cargar datos JSON en el libro de trabajo
            workbook = new Workbook("data.json", options);

            // Guarda el libro de trabajo
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


