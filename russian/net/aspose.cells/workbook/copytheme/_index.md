---
title: "Workbook.CopyTheme"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Копирует тему из другой книги"
type: docs
url: /ru/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Копирует тему из другой рабочей книги.

```csharp
public void CopyTheme(Workbook source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Рабочая книга | Исходная рабочая книга. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Создать исходную рабочую книгу (тема автоматически устанавливается при открытии файла шаблона)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            
            // Скопировать тему из исходной в целевую рабочую книгу
            destWorkbook.CopyTheme(sourceWorkbook);

            // Сохранить целевую книгу
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


