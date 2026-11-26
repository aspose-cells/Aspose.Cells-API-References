---
title: "Clase Metered"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Metered. Proporciona métodos para establecer la clave meterada"
type: docs
url: /es/net/aspose.cells/metered/
---
## Metered class

Proporciona métodos para establecer la clave medida.

```csharp
public class Metered
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Metered](metered/)() | Inicializa una nueva instancia de esta clase. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Obtiene el nombre del producto |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Establece la clave pública y privada medida. Si usted adquiere una licencia medida, al iniciar la aplicación, debe llamarse a esta API; normalmente, eso es suficiente. Sin embargo, si siempre falla la carga de datos de consumo y supera las 24 horas, la licencia se establecerá en estado de evaluación; para evitar tal caso, debe comprobar regularmente el estado de la licencia, y si está en estado de evaluación, llamar a esta API nuevamente. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Obtiene el crédito de consumo |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Obtiene el tamaño del archivo de consumo |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Verificar si Metered está licenciado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Crear una instancia de la clase Metered
            Metered metered = new Metered();

            // Establecer la clave meterada
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Obtener y mostrar el nombre del producto
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Código adicional para demostrar cómo se podría usar la instancia
            // Por ejemplo, crear un libro de trabajo y guardarlo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


