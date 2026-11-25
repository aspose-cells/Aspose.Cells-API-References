---
title: "Classe ContentTypeProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Properties.ContentTypeProperty. Rappresenta le informazioni di identificatore"
type: docs
url: /it/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Rappresenta le informazioni dell'identificatore.

```csharp
public class ContentTypeProperty
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indica se il valore può essere vuoto. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Restituisce o imposta il nome dell'oggetto. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Ottiene e imposta il tipo della proprietà. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Restituisce o imposta il valore della proprietà del tipo di contenuto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Aggiungi una nuova proprietà del tipo di contenuto
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Accedi alla proprietà appena aggiunta
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Impostazione delle proprietà
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Salva il file Excel
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


