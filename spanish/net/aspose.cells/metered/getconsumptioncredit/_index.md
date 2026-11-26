---
title: "Metered.GetConsumptionCredit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Metered. Obtiene el crédito de consumo"
type: docs
url: /es/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Obtiene el crédito de consumo

```csharp
public static decimal GetConsumptionCredit()
```

### Valor de retorno

cantidad de consumo

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Crear una instancia de la clase Metered
            Metered metered = new Metered();

            try
            {
                // Llamar al método GetConsumptionCredit de forma estática
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Mostrar el resultado
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Crear un libro de trabajo simple para demostrar el efecto (aunque GetConsumptionCredit no modifica el libro de trabajo)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Agregar la información del crédito de consumo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Guarda el libro de trabajo
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


