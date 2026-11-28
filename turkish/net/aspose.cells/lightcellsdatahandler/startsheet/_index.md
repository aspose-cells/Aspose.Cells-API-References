---
title: "LightCellsDataHandler.StartSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataHandler yöntemi. Bir çalışma sayfasını işlemeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Bir çalışma sayfasını işlemeye başlar.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | Çalışma Sayfası | hücre verilerini okumak için çalışma sayfası. |

### Dönüş Değeri

bu sayfanın hücre verilerinin işlenip işlenmeyeceği. Bu sayfayı yok saymak için false.

### Açıklamalar

Bir çalışma sayfasının hücre verileri okunmadan önce çağrılacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartSheetWithWorksheetDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                CustomLightCellsDataHandler handler = new CustomLightCellsDataHandler();
                bool result = handler.StartSheet(worksheet);

                Console.WriteLine($"StartSheet method returned: {result}");
                Console.WriteLine($"Worksheet name after StartSheet: {worksheet.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }

            workbook.Save("LightCellsDataHandlerStartSheetDemo.xlsx");
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            sheet.Name = "ModifiedByStartSheet";
            return true;
        }

        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


