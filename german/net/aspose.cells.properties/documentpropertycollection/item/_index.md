---
title: "DocumentPropertyCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentPropertyCollection‑Eigenschaft. Gibt ein DocumentProperty‑Objekt anhand des Namens der Eigenschaft zurück"
type: docs
url: /de/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Gibt ein [`DocumentProperty`](../../documentproperty/)‑Objekt anhand des Namens der Eigenschaft zurück.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Groß-/Kleinschreibung‑unabhängige Name der abzurufenden Eigenschaft. |

### Hinweise

Gibt null zurück, wenn keine Eigenschaft mit dem angegebenen Namen gefunden wird.

### Beispiele

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

            // Überprüfen Sie, ob der Wert über die Item‑Eigenschaft gesetzt wurde.
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Gibt ein [`DocumentProperty`](../../documentproperty/)‑Objekt anhand des Index zurück.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| index | Nullbasierter Index des abzurufenden [`DocumentProperty`](../../documentproperty/). |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Integrierte Dokumenteigenschaften abrufen
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Integrierte Eigenschaften setzen (nicht hinzufügen)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Zugriff auf Eigenschaften über den Item‑Indexer
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Greife über den Namen auf die Eigenschaft zu
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Eine Eigenschaft ändern
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


