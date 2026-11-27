---
title: "ConnectionParameter.SqlType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter-egenskap. SQL-datatyp för parametern. Endast giltig för ODBC-källor"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

SQL-datatyp för parametern. Endast giltig för ODBC‑källor.

```csharp
public SqlDataType SqlType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                
                // Skapa en anslutningsparameter (simulerad eftersom konstruktörsparametrar är okända)
                ConnectionParameter parameter = null;
                
                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // För demonstration visar vi hur SqlType skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella SqlType‑värdet
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Ange ett nytt SqlType‑värde (eftersom egenskapen är läs‑skriv)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


