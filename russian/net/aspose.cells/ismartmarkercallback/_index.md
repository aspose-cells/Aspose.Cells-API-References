---
title: "Интерфейс ISmartMarkerCallBack"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.ISmartMarkerCallBack. Представляет интерфейс обратного вызова для обработки смарт‑маркеров"
type: docs
url: /ru/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Представляет интерфейс обратного вызова обработки smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## Методы

| Имя | Описание |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Обратный вызов для обработки смарт‑маркера. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Реализация метода Process из интерфейса ISmartMarkerCallBack
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Пример реализации метода Process
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Создайте новый экземпляр WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            // Откройте файл шаблона (который содержит смарт‑маркеры)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Установите интерфейс обратного вызова
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Инициализируйте данные из источника данных
            // Для демонстрации мы используем простую DataTable
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Установите DataTable в качестве источника данных
            designer.SetDataSource(dataTable);

            // Обработайте смарт‑маркеры, чтобы заполнить данные в листах
            designer.Process(true);

            // Сохранить файл Excel
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


