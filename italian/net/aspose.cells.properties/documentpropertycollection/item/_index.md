---
title: "DocumentPropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentPropertyCollection. Restituisce un oggetto DocumentProperty in base al nome della proprietà"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Restituisce un oggetto [`DocumentProperty`](../../documentproperty/) in base al nome della proprietà.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà da recuperare, senza distinzione tra maiuscole e minuscole. |

### Osservazioni

Restituisce null se non viene trovata una proprietà con il nome specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // Verifica che il valore sia stato impostato usando la proprietà Item
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Restituisce un oggetto [`DocumentProperty`](../../documentproperty/) per indice.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| index | Indice basato su zero del [`DocumentProperty`](../../documentproperty/) da recuperare. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni le proprietà del documento predefinite
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Imposta le proprietà predefinite (non Add)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Accedi alle proprietà usando l'indicizzatore Item
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Accede alla proprietà per nome
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Modifica una proprietà
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


