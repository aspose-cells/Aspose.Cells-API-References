---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Представляет оценку количества строк в документе"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Представляет оценку количества строк в документе.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Примечания

Aspose.Cells не обновляет это свойство при изменении документа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Отобразить текущее значение Lines (оценка количества строк в документе)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Установите новое значение свойства Lines
            properties.Lines = 150;
            
            // Добавьте некоторое содержимое, чтобы продемонстрировать назначение свойства
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Сохраните книгу
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Примечание: Свойство Lines является оценочным и не будет автоматически обновляться при изменении реального содержимого
            // Оно в основном используется для целей метаданных документа
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


