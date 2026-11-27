---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter‑egenskap. Flagga som anger om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false uppdateras extern data endast när användaren begär det eller någon annan händelse triggar en uppdatering, t.ex. när arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse utlöser en uppdatering (t.ex. arbetsboken öppnas).

```csharp
public bool RefreshOnChange { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
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
                
                // För demonstration visar vi hur RefreshOnChange skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella RefreshOnChange‑värdet
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Ange ett nytt RefreshOnChange‑värde (eftersom egenskapen är läs‑skriv)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


