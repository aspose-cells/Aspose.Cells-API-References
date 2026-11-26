---
title: "CustomProperty.StringValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomProperty. Devuelve o establece el valor de la propiedad personalizada"
type: docs
url: /es/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Devuelve o establece el valor de la propiedad personalizada.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Observaciones

NOTA: Este miembro ahora está obsoleto. En su lugar, por favor use la propiedad CustomProperty.Value. Esta propiedad será eliminada 12 meses después desde junio de 2010. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una propiedad personalizada con un valor de cadena
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Recuperar la propiedad personalizada
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Mostrar la propiedad StringValue (operación de lectura)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Establecer un nuevo valor para la propiedad StringValue
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Guarda el libro de trabajo
                workbook.Save("StringValueDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


