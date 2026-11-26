---
title: "Класс PivotShowValuesSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotShowValuesSetting. Представляет настройки отображения значений, когда используется вычисление ShowDataAs"
type: docs
url: /ru/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Представляет настройки отображения значений, когда используется вычисление ShowDataAs.

```csharp
public class PivotShowValuesSetting
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Представляет базовое поле для вычисления ShowDataAs, когда вычисление ShowDataAs используется. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Получает подпись базового поля сводки. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Получает подпись элемента сводки в базовом поле. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Представляет пользовательский индекс элемента сводки в базовом поле, когда используется вычисление ShowDataAs. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Представляет тип базового элемента сводки в базовом поле, когда используется вычисление ShowDataAs. Поскольку PivotItemPosition.Custom доступен только для чтения, если необходимо установить PivotItemPosition.Custom, пожалуйста, задайте атрибут PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Представляет способ отображения значений поля данных в отчете сводки. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Получает и задает способ отображения значений поля данных в отчете сводки. |

## Поля

| Имя | Описание |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Особый индекс базового элемента: использовать следующий элемент сводки. Действительно для вычислений "Show Values As"; применимо в Excel 2010 и более новых версиях. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Особый индекс базового элемента: использовать предыдущий элемент сводки. Действительно для вычислений "Show Values As"; применимо в Excel 2010 и более новых версиях. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Доступ к полю данных
            PivotField dataField = pivotTable.DataFields[0];

            // Доступ к свойству ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Установить свойства PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


