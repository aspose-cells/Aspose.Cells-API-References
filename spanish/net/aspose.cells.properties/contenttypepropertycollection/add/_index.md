---
title: "ContentTypePropertyCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ContentTypePropertyCollection. Agrega información de propiedades de tipo de contenido"
type: docs
url: /es/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Agrega información de la propiedad de tipo de contenido.

```csharp
public int Add(string name, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad del tipo de contenido. |
| valor | String | El valor de la propiedad del tipo de contenido. |

### Ejemplos

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

### Ver también

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Agrega información de la propiedad de tipo de contenido.

```csharp
public int Add(string name, string value, string type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad del tipo de contenido. |
| valor | String | El valor de la propiedad del tipo de contenido. |
| type | String | El tipo de la propiedad del tipo de contenido. |

### Ejemplos

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

### Ver también

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


