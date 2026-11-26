---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLoadOptions. Indica si se importa cada atributo del objeto JsonObject como una hoja de cálculo cuando todos los nodos hijos son nodos de matriz"
type: docs
url: /es/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Indica si se importa cada atributo del objeto JsonObject como una hoja de cálculo cuando todos los nodos hijos son nodos de matriz.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga JSON con MultipleWorksheets habilitado
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // Cargar archivo JSON en el libro de trabajo con las opciones especificadas
            Workbook workbook = new Workbook("example.json", options);
            
            // Acceder a los datos de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Mostrar algunos valores de ejemplo del JSON cargado
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Ver también

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


