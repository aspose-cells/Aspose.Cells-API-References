---
title: "Klass ConnectionParameter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ConnectionParameter-klass. Anger egenskaper för alla parametrar som används med externa datakopplingar. Parametrar är giltiga för ODBC- och webbfrågor"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Anger egenskaper för alla parametrar som används med externa datakopplingar. Parametrar är giltiga för ODBC- och webbfrågor.

```csharp
public class ConnectionParameter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Cellreferens som anger vilket cells värde som ska användas för frågeparametern. Används endast när parameterType är cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Namnet på parametern. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Prompt-sträng för parametern. Presenteras för kalkylarksanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan den externa datan uppdateras. Används endast när parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse utlöser en uppdatering (t.ex. arbetsboken öppnas). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | SQL-datatyp för parametern. Endast giltig för ODBC‑källor. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av {boolean, double, integer, or string} specificeras. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Icke-heltal numeriskt värde, Integer‑värde, String‑värde eller Boolean‑värde att använda som frågeparameter. Används endast när parameterType är value. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en anslutningsparameter med reflection eftersom konstruktorn inte är publik
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Ställ in grundläggande egenskaper
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Visa parameterinformation
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Spara arbetsboken
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


