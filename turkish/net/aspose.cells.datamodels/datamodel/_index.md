---
title: "Sınıf DataModel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataModels.DataModel sınıfı. Veri modelini temsil eder"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Veri modelini temsil eder.

```csharp
public class DataModel
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Veri modelindeki tabloların tüm ilişkilerini alır. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Veri modelindeki tüm tabloları alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yeni bir örnek oluşturmaktansa çalışma kitabından DataModel'i al
            DataModel dataModel = workbook.DataModel;

            // Tablo ve ilişkilerin (yalnızca okunabilir özellikler) erişimini göster
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Not: Tablolar ve İlişkiler yalnızca okunabilir koleksiyonlar olduğundan,
            // sadece mevcut öğelere erişebiliriz ancak doğrudan değiştiremeziz

            // Çalışma kitabını kaydet (DataModel genellikle Aspose.Cells tarafından dahili olarak kullanılır)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


