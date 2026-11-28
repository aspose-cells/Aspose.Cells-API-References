---
title: "DataModel.Relationships"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModel özelliği. Veri modelindeki tabloların tüm ilişkilerini alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Veri modelindeki tabloların tüm ilişkilerini alır.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Çalışma kitabından DataModel'e erişin
                DataModel dataModel = workbook.DataModel;

                // Relationships özelliğinin mevcut değerini gösterin (yalnızca okunabilir)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Varsa ilişkiler arasında yineleme yapın
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


