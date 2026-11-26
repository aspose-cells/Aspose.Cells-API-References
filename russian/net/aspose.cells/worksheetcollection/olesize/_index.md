---
title: "WorksheetCollection.OleSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Получает и задаёт отображаемый размер, когда файл Workbook используется как объект Ole"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Получает и задает отображаемый размер, когда файл Workbook используется как объект OLE.

```csharp
public object OleSize { get; set; }
```

### Примечания

Null означает отсутствие настройки размера ole.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить размер OLE для коллекции листов
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Получить доступ и отобразить свойства размера OLE
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Сохраните книгу
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


