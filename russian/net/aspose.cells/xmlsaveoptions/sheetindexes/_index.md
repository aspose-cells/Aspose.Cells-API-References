---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlSaveOptions. Представляет индексы экспортируемых листов"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Представляет индексы экспортируемых листов.

```csharp
public int[] SheetIndexes { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Заполните некоторыми данными все листы
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Создайте экземпляр XmlSaveOptions
            XmlSaveOptions options = new XmlSaveOptions();

            // Изначально экспортировать все листы (SheetIndexes равно null)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Установите экспорт только первого и третьего листов (индексы 0 и 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Сохранить только с выбранными листами
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Изменить на экспорт только второго листа (индекс 1)
            options.SheetIndexes = new int[] { 1 };

            // Сохранить с другим выбором листов
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Установите SheetIndexes в null, чтобы экспортировать все листы
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### См. также

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


