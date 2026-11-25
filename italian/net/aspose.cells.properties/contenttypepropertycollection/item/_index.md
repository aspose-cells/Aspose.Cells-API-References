---
title: "ContentTypePropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ContentTypePropertyCollection. Ottiene la proprietà del tipo di contenuto per l'indice specifico"
type: docs
url: /it/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Ottiene la proprietà del tipo di contenuto per l'indice specifico.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La proprietà del tipo di contenuto

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi proprietà del tipo di contenuto e dimostra l'uso della proprietà Item
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Accedi alle proprietà usando l'indicizzatore Item
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Ottiene la proprietà del tipo di contenuto per nome della proprietà.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà. |

### Valore di ritorno

La proprietà del tipo di contenuto

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi proprietà del tipo di contenuto
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Accedi alla proprietà usando l'indicizzatore Item
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Modifica i valori della proprietà
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Salva cartella di lavoro
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


