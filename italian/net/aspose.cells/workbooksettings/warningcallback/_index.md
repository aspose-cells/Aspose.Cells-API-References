---
title: "WorkbookSettings.WarningCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta il callback di avviso"
type: docs
url: /it/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Ottiene o imposta il callback di avviso.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta il callback di avviso
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Crea un foglio di lavoro con uno scenario di avviso potenziale (intervallo denominato duplicato)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Questo genererà un avviso sul nome duplicato
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Salva la cartella di lavoro (genererà il callback di avviso)
            workbook.Save("WarningCallbackExample.xlsx");
        }
    }

    public class WarningCallbackImplementation : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
        }
    }
}
```

### Vedi anche

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


