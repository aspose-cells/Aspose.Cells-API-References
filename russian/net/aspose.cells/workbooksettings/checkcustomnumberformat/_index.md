---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, следует ли проверять пользовательский числовой формат при установке Style.Custom"
type: docs
url: /ru/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Указывает, проверять ли пользовательский числовой формат при установке Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Сначала задайте корректный пользовательский числовой формат
            style.Custom = "#,##0.00";
            
            // Включить строгую проверку
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Попытка установить недопустимый пользовательский числовой формат
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


