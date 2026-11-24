---
title: "ContentTypePropertyCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypePropertyCollection-Eigenschaft. Ruft die Content-Type-Eigenschaft anhand des angegebenen Index ab"
type: docs
url: /de/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Ruft die Content-Type-Eigenschaft anhand des angegebenen Index ab.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die Content-Type-Eigenschaft

### Beispiele

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
            
            // Fügen Sie Content-Type-Eigenschaften hinzu und demonstrieren Sie die Verwendung der Item-Eigenschaft
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Zugriff auf Eigenschaften über den Item‑Indexer
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Ruft die Content-Type-Eigenschaft anhand des Eigenschaftsnamens ab.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Property-Name. |

### Rückgabewert

Die Content-Type-Eigenschaft

### Beispiele

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
            
            // Fügen Sie eine Content-Type-Eigenschaft hinzu
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Greifen Sie auf die Eigenschaft über den Item-Indexer zu
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Ändern Sie Eigenschaftswerte
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Arbeitsmappe speichern.
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


