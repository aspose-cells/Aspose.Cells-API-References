---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Özelliğin adıyla bir DocumentProperty nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Özelliğin adıyla bir [`DocumentProperty`](../../documentproperty/) nesnesi döndürür.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Alınacak özelliğin büyük/küçük harfe duyarsız adı. |

### Açıklamalar

Özelliklerin dize adları, [`BuiltInDocumentPropertyCollection`](../) üzerinden kullanılabilen tiplenmiş özelliklerin adlarıyla eşleşir.

Belgede bulunmayan bir özelliği talep ederseniz, ancak özelliğin adı geçerli bir yerleşik ad olarak tanınıyorsa, yeni bir [`DocumentProperty`](../../documentproperty/) oluşturulur, koleksiyona eklenir ve döndürülür. Yeni oluşturulan özelliğe, yerleşik özelliğin tipine bağlı olarak (boş dize, sıfır, false veya DateTime.MinValue) varsayılan bir değer atanır.

Belgede bulunmayan bir özelliği talep ederseniz ve ad bir yerleşik ad olarak tanınmazsa, null döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Uygun yöntemi kullanarak bir yerleşik belge özelliği ayarlayın
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Özellik değerine erişin ve yazdırın
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyin ve özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


