---
title: "ContentTypePropertyCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ContentTypePropertyCollection. Ajoute des informations de propriété de type de contenu"
type: docs
url: /fr/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Ajoute des informations de propriété de type de contenu.

```csharp
public int Add(string name, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété de type de contenu. |
| valeur | String | La valeur de la propriété de type de contenu. |

### Exemples

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

### Voir aussi

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Ajoute des informations de propriété de type de contenu.

```csharp
public int Add(string name, string value, string type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété de type de contenu. |
| valeur | String | La valeur de la propriété de type de contenu. |
| type | String | Le type de la propriété de type de contenu. |

### Exemples

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

### Voir aussi

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


