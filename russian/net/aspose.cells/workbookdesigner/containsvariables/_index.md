---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Указывает, содержит ли первый лист пользовательские переменные"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Указывает, содержит ли первый лист пользовательские переменные.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство WorkbookDesigner.VariablesWorksheetName. Это свойство будет удалено через 3 месяца, начиная с сентября 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте экземпляр WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Отобразите текущее значение свойства ContainsVariables
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Установите свойство ContainsVariables в true
                designer.ContainsVariables = true;

                // Отобразить обновлённое значение
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Сохранить результат
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
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


