---
title: "DataModelRelationshipCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelRelationshipCollection özelliği. İlişkiyi alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

İlişkiyi alır.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun (boş veri modeli)
            Workbook workbook = new Workbook();

            try
            {
                // Çalışma kitabından DataModelRelationshipCollection'ı alın (veri modeli yoksa null olabilir)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // Item (indeksleyici) özelliğini kullanarak ilk ilişkiyi okuyun
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Çalışma kitabını kaydedin (isteğe bağlı, sadece kodun uçtan uca çalıştığını göstermek için)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


