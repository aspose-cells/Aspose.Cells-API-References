---
title: "WorkbookSettings.WarningCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает обратный вызов предупреждения"
type: docs
url: /ru/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Получает или задаёт обратный вызов предупреждения.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить обратный вызов предупреждения
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Создайте лист с потенциальным сценарием предупреждения (дублируемый именованный диапазон)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Это вызовет предупреждение о дублирующемся имени
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Сохраните книгу (это вызовет обратный вызов предупреждения)
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

### См. также

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


