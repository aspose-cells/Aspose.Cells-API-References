---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Получает и задает имя листа, содержащего переменные smart marker"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Получает и задает имя листа, содержащего переменные smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();

                // Добавьте лист с именем "Variables" для демонстрации свойства
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Создайте экземпляр WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Отобразите текущее значение VariablesWorksheetName
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Установите новое значение для VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Добавьте другой лист с smart markers
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Обработайте smart markers
                designer.Process();

                // Сохраните книгу
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


