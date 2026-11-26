---
title: "CustomProperty.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomProperty. Devuelve o establece el valor de la propiedad personalizada"
type: docs
url: /es/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Devuelve o establece el valor de la propiedad personalizada.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una propiedad personalizada con un valor de cadena largo
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Obtener y mostrar el valor de la propiedad personalizada
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Recargar el libro de trabajo para verificar que la propiedad persista
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Verificar que el valor sea el mismo después de cargar
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Ver también

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


