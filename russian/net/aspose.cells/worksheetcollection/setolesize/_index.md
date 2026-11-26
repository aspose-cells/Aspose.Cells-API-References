---
title: "WorksheetCollection.SetOleSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorksheetCollection метод. Устанавливает отображаемый размер, когда файл Workbook используется как объект Ole"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Устанавливает отображаемый размер, когда файл книги используется как объект OLE.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| endRow | Int32 | Индекс конечной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примечания

Этот метод обычно используется для корректировки размера отображения в файлах ppt или doc.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить размер OLE для листов
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверить размер OLE
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


