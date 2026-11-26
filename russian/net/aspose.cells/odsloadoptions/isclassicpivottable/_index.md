---
title: "OdsLoadOptions.IsClassicPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsLoadOptions. Указывает, является ли сводная таблица классической"
type: docs
url: /ru/net/aspose.cells/odsloadoptions/isclassicpivottable/
---
## OdsLoadOptions.IsClassicPivotTable property

Указывает, является ли сводная таблица классической.

```csharp
public bool IsClassicPivotTable { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
    {
        public static void Run()
        {
            // Создать пример ODS файла со сводной таблицей
            CreateSampleOdsWithPivotTable();

            // Загрузить с IsClassicPivotTable, установленным в true
            OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
            loadOptionsTrue.IsClassicPivotTable = true;
            
            Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
            Console.WriteLine("Loaded with IsClassicPivotTable = true");
            Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);

            // Загрузить с IsClassicPivotTable, установленным в false
            OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
            loadOptionsFalse.IsClassicPivotTable = false;
            
            Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
            Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
            Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
        }

        private static void CreateSampleOdsWithPivotTable()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполнить примерными данными
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Electronics";
            cells["A3"].Value = "Clothing";
            cells["A4"].Value = "Books";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 800;
            cells["B4"].Value = 200;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки (Category)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить поле данных (Sales) и задать отображаемое имя
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";

            // Сохранить как ODS
            workbook.Save("SamplePivot.ods", SaveFormat.Ods);
        }
    }
}
```

### См. также

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


