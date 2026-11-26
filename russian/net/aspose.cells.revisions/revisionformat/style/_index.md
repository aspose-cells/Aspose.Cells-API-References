---
title: "RevisionFormat.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionFormat. Получает применённый стиль"
type: docs
url: /ru/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Получает применённый стиль.

```csharp
public Style Style { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу (отслеживание изменений включено по умолчанию при внесении изменений)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте данные и форматирование, чтобы создать ревизию
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Создать стиль и применить его к ячейке
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Получите доступ к ревизиям через RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Отобразите текущие свойства стиля из ревизии
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Примечание: свойство Style является только для чтения в RevisionFormat, поэтому мы не можем изменить его напрямую
                        // Чтобы изменить форматирование, нам нужно напрямую изменить стиль ячейки
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


