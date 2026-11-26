---
title: "Workbook.Combine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Объединяет другой объект Workbook"
type: docs
url: /ru/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Объединяет другой объект Workbook.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| secondWorkbook | Рабочая книга | Другой объект Workbook. |

### Примечания

Объедините файлы Excel, ODS, CSV и другие в один файл.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Создайте исходную рабочую книгу
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Объедините рабочие книги
            destWorkbook.Combine(sourceWorkbook);

            // Сохраните объединённую рабочую книгу
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


