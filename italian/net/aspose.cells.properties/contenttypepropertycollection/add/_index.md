---
title: "ContentTypePropertyCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ContentTypePropertyCollection. Aggiunge informazioni sulla proprietà di tipo contenuto"
type: docs
url: /it/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Aggiunge informazioni sulla proprietà del tipo di contenuto.

```csharp
public int Add(string name, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà del tipo di contenuto. |
| valore | String | Il valore della proprietà del tipo di contenuto. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
            ctps.Add("CustomProperty1", "SampleValue1");
            ctps.Add("CustomProperty2", "SampleValue2");
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Aggiunge informazioni sulla proprietà del tipo di contenuto.

```csharp
public int Add(string name, string value, string type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà del tipo di contenuto. |
| valore | String | Il valore della proprietà del tipo di contenuto. |
| type | String | Il tipo della proprietà del tipo di contenuto. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add("propertyName", "propertyValue", "string");
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


