---
title: "DocumentProperty.ToBool"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentProperty. Restituisce il valore della proprietà come bool"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Restituisce il valore della proprietà come bool.

```csharp
public bool ToBool()
```

### Osservazioni

Genera un'eccezione se il tipo della proprietà non è PropertyType.Boolean.

### Esempi

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

            // Aggiungi una proprietà personalizzata del documento di tipo booleano
            customProperties.Add("IsApproved", true);
            
            // Ottieni la proprietà e converti in bool usando ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


