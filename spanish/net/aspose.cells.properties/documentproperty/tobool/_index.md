---
title: "DocumentProperty.ToBool"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentProperty. Devuelve el valor de la propiedad como bool"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Devuelve el valor de la propiedad como bool.

```csharp
public bool ToBool()
```

### Observaciones

Lanza una excepción si el tipo de la propiedad no es PropertyType.Boolean.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agregue una propiedad personalizada del documento booleana
            customProperties.Add("IsApproved", true);
            
            // Obtenga la propiedad y conviértala a bool usando ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


