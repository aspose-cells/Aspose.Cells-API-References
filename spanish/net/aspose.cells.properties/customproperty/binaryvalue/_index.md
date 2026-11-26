---
title: "CustomProperty.BinaryValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomProperty. Obtiene y establece el valor binario de la propiedad personalizada"
type: docs
url: /es/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Obtiene y establece el valor binario de la propiedad personalizada.

```csharp
public byte[] BinaryValue { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una propiedad personalizada con un valor de ejemplo
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Recuperar la propiedad personalizada
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Mostrar el Name y el Value de la propiedad personalizada
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // NOTA: La reflexión de CustomProperty no incluye una propiedad BinaryValue.
                // El valor basado en cadena disponible se accede a través de la propiedad 'Value'.

                // Guardar el libro de trabajo (opcional)
                workbook.Save("BinaryValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


