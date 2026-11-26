---
title: "Metered.IsMeteredLicensed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Metered. Verifica si metered está licenciado"
type: docs
url: /es/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Verificar si Metered está licenciado

```csharp
public static bool IsMeteredLicensed()
```

### Valor de retorno

Verdadero o falso

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de Metered
            Metered metered = new Metered();

            try
            {
                // Verificar si la licencia metered está aplicada
                bool isLicensed = Metered.IsMeteredLicensed();

                // Mostrar el resultado
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Agregar el resultado a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


