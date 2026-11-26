---
title: "Worksheet.CustomProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de la hoja de cálculo. Obtiene un objeto que representa la información de identificación asociada a una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Obtiene un objeto que representa la información de identificador asociada a una hoja de cálculo.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Observaciones

Worksheet.CustomProperties proporciona un mecanismo preferido para almacenar datos arbitrarios. Soporta componentes de documentos de terceros heredados, así como aquellas situaciones que requieren estrictamente partes binarias.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar propiedades personalizadas a la hoja de cálculo
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Mostrar el recuento de propiedades personalizadas
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Acceder y mostrar los valores de las propiedades
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


