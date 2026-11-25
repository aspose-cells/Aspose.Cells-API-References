---
title: "Enum PropertyType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Properties.PropertyType. Specifica il tipo di dato di una proprietà del documento"
type: docs
url: /it/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Specifica il tipo di dato di una proprietà del documento.

```csharp
public enum PropertyType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Boolean | `0` | La proprietà è un valore booleano. |
| DateTime | `1` | La proprietà è un valore data/ora. |
| Double | `2` | La proprietà è un numero a virgola mobile. |
| Number | `3` | La proprietà è un numero intero. |
| String | `4` | La proprietà è un valore stringa. |
| Blob | `5` | La proprietà è un array di byte. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta alcune proprietà integrate
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Accedi alle proprietà personalizzate del documento
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Aggiungi proprietà personalizzate di diversi tipi
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Recupera e visualizza le proprietà personalizzate
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Salva la cartella di lavoro
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


