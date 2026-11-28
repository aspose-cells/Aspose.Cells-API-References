---
title: "ContentTypePropertyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypePropertyCollection özelliği. Belirli bir indeksle içerik türü özelliğini alır"
type: docs
url: /tr/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Belirli bir indeksle içerik türü özelliğini alır.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

İçerik türü özelliği

### Örnekler

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
            
            // İçerik türü özelliklerini ekleyin ve Item özelliği kullanımını gösterin
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Özelliklere Item dizinleyicisiyle eriş
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Özellik adıyla içerik türü özelliğini alır.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Özellik adı. |

### Dönüş Değeri

İçerik türü özelliği

### Örnekler

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
            
            // İçerik türü özelliği ekle
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Item dizinleyicisini kullanarak özelliğe erişin
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Özellik değerlerini değiştirin
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Çalışma kitabını kaydet
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


