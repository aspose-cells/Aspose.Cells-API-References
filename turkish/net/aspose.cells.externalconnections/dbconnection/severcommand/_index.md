---
title: "DBConnection.SeverCommand"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci bir komut metni dizesi belirtir. ODBC bağlantıları için serverCommand genellikle komuttan daha geniş bir sorgudur; önceki sorguda WHERE koşulu bulunmaz. Bu iki komut (Command ve ServerCommand) temelinde parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metin dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu bulunmaz). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir.

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen ExternalConnection.SecondCommand özelliğini kullanın. Bu yöntem, Ekim 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class DBConnectionPropertySeverCommandDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (connection is DBConnection dbConn)
                {
                    dbConn.Name = dbConn.Name.Replace("c:\\", "d:\\");
                    dbConn.SourceFile = dbConn.SourceFile.Replace("c:\\", "d:\\");
                    dbConn.ConnectionInfo = dbConn.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
                    dbConn.Command = dbConn.Command.Replace("c:\\", "d:\\");
                    
                    if (!string.IsNullOrEmpty(dbConn.SeverCommand))
                        dbConn.SeverCommand = dbConn.SeverCommand.Replace("c:\\", "d:\\");
                }
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


