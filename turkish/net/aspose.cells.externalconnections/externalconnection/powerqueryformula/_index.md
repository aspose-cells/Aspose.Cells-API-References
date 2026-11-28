---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. power query formula tanımını alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Power query formülünün tanımını alır.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // PowerQueryFormula'ı göstermek için veri bağlantılarına sahip mevcut bir çalışma kitabını yükle
            workbook = new Workbook("example.xlsx");
            
            // Mevcut bir bağlantıya erişin (çalışma kitabının en az bir bağlantısı olduğunu varsayarak)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // PowerQueryFormula özelliğine erişin
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


