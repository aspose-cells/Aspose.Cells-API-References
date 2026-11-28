---
title: "ExternalConnection.ConnectionDescription"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bu bağlantı için kullanıcı açıklamasını belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Bu bağlantı için kullanıcı açıklamasını belirtir.

```csharp
public string ConnectionDescription { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Örnek veri içeren bir çalışma sayfası ekle
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // Harici bir bağlantı oluşturmak için bir pivot tablo oluştur
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Pivot tablodan dış bağlantıyı alın
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // İlk ConnectionDescription değerini göster
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // Yeni bir açıklama ayarla (okunabilir-yazılabilir olduğu için)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // Açıklamayı temizle
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // Değiştirilmiş bağlantı ile çalışma kitabını kaydet
                workbook.Save("ConnectionDescriptionDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


