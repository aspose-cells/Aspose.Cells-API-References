---
title: "QueryTableCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTableCollection özelliği. Belirli indeksle sorgu tablosunu alır"
type: docs
url: /tr/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Belirli bir indeksle QueryTable'ı alır.

```csharp
public QueryTable this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Sorgu tablosu

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // QueryTableCollection'a eriş
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Herhangi bir QueryTable olup olmadığını kontrol et
                if (queryTables.Count > 0)
                {
                    // Item özelliğini kullanarak ilk QueryTable'a eriş
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // QueryTable'ın bazı özelliklerini göster
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("QueryTableItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


