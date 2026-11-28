---
title: "ExternalConnection.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Dış bağlantı DataSource türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Harici bağlantının DataSource türünü alır veya ayarlar.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.SourceType özelliğini kullanın. Bu özellik, Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Geçerli Type değerini göster (okuma işlemi)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Yeni bir Type değeri ayarla (okuma-yazma olduğu için)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Ayar yeteneğini göstermek için olası değerler arasında dolaş
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


