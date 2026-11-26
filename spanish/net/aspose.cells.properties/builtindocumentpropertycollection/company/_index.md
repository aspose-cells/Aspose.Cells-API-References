---
title: "BuiltInDocumentPropertyCollection.Company"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la propiedad de la empresa"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Obtiene o establece la propiedad de la empresa.

```csharp
public string Company { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCompanyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer propiedades de documento incorporadas incluyendo Company
            workbook.BuiltInDocumentProperties.Title = "Annual Report";
            workbook.BuiltInDocumentProperties.Company = "Contoso Ltd";
            
            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx");
            
            // Mostrar las propiedades establecidas
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties.Title);
            Console.WriteLine("Company: " + workbook.BuiltInDocumentProperties.Company);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


