---
title: "DocumentProperty.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentProperty. Ottiene il tipo di dati della proprietà"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Ottiene il tipo di dati della proprietà.

```csharp
public PropertyType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà personalizzate del documento (non integrate)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Aggiungi proprietà personalizzate con tipi diversi
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // Accedi a una proprietà specifica e verifica il suo tipo
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### Vedi anche

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


