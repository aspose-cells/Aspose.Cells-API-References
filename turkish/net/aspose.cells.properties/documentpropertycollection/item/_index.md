---
title: "DocumentPropertyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentPropertyCollection özelliği. Özelliğin adıyla bir DocumentProperty nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Özelliğin adıyla bir [`DocumentProperty`](../../documentproperty/) nesnesi döndürür.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Alınacak özelliğin büyük/küçük harfe duyarsız adı. |

### Açıklamalar

Belirtilen ada sahip bir özellik bulunamazsa null döndürür.

### Örnekler

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

            // Değerin Item özelliği kullanılarak ayarlandığını doğrulayın
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

İndexe göre bir [`DocumentProperty`](../../documentproperty/) nesnesi döndürür.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| index | Alınacak [`DocumentProperty`](../../documentproperty/) nesnesinin sıfır tabanlı indeksi. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özelliklerini al
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Yerleşik özellikleri ayarla (Ekleme değil)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Özelliklere Item dizinleyicisiyle eriş
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Ada göre özelliğe eriş.
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Bir özelliği değiştir
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


