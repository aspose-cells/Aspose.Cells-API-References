---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Om denna workbook innehåller externa länkar till en annan datakälla kommer Aspose.Cells att försöka hämta den senaste datan från angivna källor"
type: docs
url: /sv/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Om den här arbetsboken innehåller externa länkar till andra datakällor, kommer Aspose.Cells att försöka hämta den senaste datan från angivna källor.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Workbooks som kommer att användas för att uppdatera data för externa länkar som refereras av denna workbook. Matchningen av dessa workbooks med externa länkar bestäms av [`FileName`](../filename/) och [`DataSource`](../../externallink/datasource/). Så se till att [`FileName`](../filename/) har angetts med rätt värde för varje workbook så att de kan länkas till motsvarande externa länk. |

### Anmärkningar

Om motsvarande extern länk inte kan hittas för en workbook, kommer den workbook att ignoreras. Så när du senare sätter en formel med en ny extern länk som du avser att länka den ignorerade workbooken till, kan länken inte utföras förrän du anropar den här metoden igen med de workbooks.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en huvud‑workbook med externa referenser
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Skapa extern workbook som ska länkas
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Anropa UpdateLinkedDataSource med den externa workbook‑arrayen
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Beräkna formler för att uppdatera referensen
                mainWorkbook.CalculateFormula();

                // Visa det uppdaterade värdet
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Spara resultatet
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


