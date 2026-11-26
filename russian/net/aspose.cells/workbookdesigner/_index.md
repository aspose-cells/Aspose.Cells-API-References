---
title: "Класс WorkbookDesigner"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WorkbookDesigner. Инкапсулирует объект, представляющий дизайнерскую электронную таблицу"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Инкапсулирует объект, представляющий проектную электронную таблицу.

```csharp
public class WorkbookDesigner
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Инициализирует новый экземпляр класса `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Инициализирует новый экземпляр класса `WorkbookDesigner`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Указывает, следует ли вычислять формулы. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Получает и задает интерфейс обратного вызова обработки smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Указывает, содержит ли первый лист пользовательские переменные. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Указывает, содержит ли верхний/нижний колонтитул smart markers и должен ли он обрабатываться совместно. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Указывает, обрабатывается ли smart marker построчно. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Указывает, повторяются ли формулы с строкой подытога. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Указывает, сортировать ли источник данных. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Если TRUE, будет вставлен Null, если значение равно ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Указывает, будут ли обновляться ссылки в других листах. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Получает и задает имя листа, содержащего переменные smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Получает и задает объект [`Workbook`](./workbook/). |

## Методы

| Имя | Описание |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Очищает все источники данных. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Возвращает коллекцию смарт‑маркировок в электронной таблице. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Обрабатывает смарт‑маркировки и заполняет значения источника данных. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Обрабатывает смарт‑маркировки и заполняет значения источника данных. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Обрабатывает смарт‑маркировки и заполняет значения источника данных. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Устарело.**) Обрабатывает смарт‑маркировки и заполняет значения источника данных. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Устанавливает источник данных объекта DataSet. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Устанавливает источник данных объекта DataTable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Устанавливает источник данных объекта DataView. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Устанавливает источник данных объекта OleDbConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Устанавливает источник данных объекта SqlConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Устанавливает источник данных объекта DataView и привязывает его к имени источника данных. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Устанавливает источник данных объекта [`ICellsDataTable`](../icellsdatatable/). |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Устанавливает привязку данных к переменной. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Устанавливает источник данных объекта IDataReader. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Устанавливает значение строки JSON в качестве источника данных смарт‑маркировок. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // Создать объект WorkbookDesigner
            WorkbookDesigner wd = new WorkbookDesigner();

            // Откройте файл шаблона (который содержит смарт‑маркировки)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Инициализируйте данные из источника данных
            DataSet ds = new DataSet();
            // Добавьте данные в набор данных (это лишь пример, замените реальным источником данных)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Установите набор данных в качестве источника данных
            wd.SetDataSource(ds);

            // Обработайте смарт‑маркеры, чтобы заполнить данные в листах
            wd.Process(true);

            // Сохранить файл Excel
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Демонстрация других свойств
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Очистить источник данных
            wd.ClearDataSource();

            // Установите источник данных различными способами
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Обработайте смарт‑маркировки снова
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Сохраните файл Excel снова
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


