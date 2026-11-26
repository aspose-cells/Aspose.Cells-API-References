---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IPageSavingCallback. Управлять/Указывать, что страница завершена для вывода"
type: docs
url: /ru/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Контролировать/индицировать завершение вывода страницы.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| args | PageEndSavingArgs | Информация о странице завершает процесс сохранения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Создать новую книгу и заполнить данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для создания нескольких страниц при рендеринге
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Создать параметры сохранения PDF с пользовательским обратным вызовом сохранения страниц
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Сохранить книгу с реализацией обратного вызова
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Отобразить информацию о завершении сохранения страницы
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Здесь можно добавить операции с файлами или другую постобработку
                // args.HasMorePages показывает, будут ли обрабатываться дополнительные страницы
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Требуемая реализация интерфейса
            }
        }
    }
}
```

### См. также

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


