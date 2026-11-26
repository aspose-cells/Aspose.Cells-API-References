---
title: "Metered.GetProductName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Metered. Obtiene el nombre del producto"
type: docs
url: /es/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Obtiene el nombre del producto

```csharp
public string GetProductName()
```

### Valor de retorno

nombre del producto

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Crear una instancia metered
            Metered metered = new Metered();
            
            // Establecer claves metered (reemplazar con claves reales)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Obtener y mostrar el nombre del producto
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Demostrar uso básico con una hoja de cálculo simple
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


