---
title: "Metered.GetConsumptionQuantity"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Metered. Obtiene el tamaño del archivo de consumo"
type: docs
url: /es/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Obtiene el tamaño del archivo de consumo

```csharp
public static decimal GetConsumptionQuantity()
```

### Valor de retorno

cantidad de consumo

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Crear una instancia metered
            Metered metered = new Metered();

            try
            {
                // Establecer claves medidas (reemplazar con claves reales en uso real)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Obtener cantidad de consumo
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Mostrar el resultado
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Crear un libro de trabajo para demostrar el uso medido
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Agregar algunos datos para mostrar que el libro de trabajo funciona
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Guarda el libro de trabajo
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


