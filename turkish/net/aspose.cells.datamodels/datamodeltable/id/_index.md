---
title: "DataModelTable.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelTable özelliği. Veri modeli tablosunun kimliğini alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Veri modeli tablosunun kimliğini alır.

```csharp
public string Id { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Bir ListObject (tablo) oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // DataModelTable'ı alın (çalışma kitabında yalnızca okunur)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Mevcut Id değerini gösterin
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Not: Id özelliği yalnızca okunabilir, bu yüzden ayarlayamayız
            // Bu, mevcut Id'ye nasıl erişileceğini ve kullanılacağını gösterir

            // Örnek kullanım: Birden fazla tabloyla çalışırken tablo ID'lerini karşılaştırın
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


