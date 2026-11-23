---
title: "类 PivotGlobalizationSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Settings.PivotGlobalizationSettings 类。表示数据透视表的全球化设置"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

表示透视表的全局化设置。

```csharp
public class PivotGlobalizationSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [GetFormatOfDayGroup](../../aspose.cells.settings/pivotglobalizationsettings/getformatofdaygroup/)() | 获取数据透视日分组的数字格式。仅在按天对数据透视字段进行分组时使用。默认值为 "d-MMM"； |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | 获取数据透视字段的显示名称。默认格式为 "Sum Of Field"。 |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | 获取 12 个月的所有短格式字符串。 |
| virtual [GetTextOf24Hours](../../aspose.cells.settings/pivotglobalizationsettings/gettextof24hours/)() | 获取 24 小时的所有本地格式字符串。默认值为 12 AM、1 AM、2 AM、3 AM、4 AM、5 AM、6 AM、7 AM、8 AM、9 AM、10 AM、11 AM、12 PM、1 PM、2 PM、3 PM、4 PM、5 PM、6 PM、7 PM、8 PM、9 PM、10 PM、11 PM。 |
| virtual [GetTextOf4Quarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quarters/)() | 获取 4 个季度的本地文本。 |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | (**已废弃。**) 获取 4 个季度的本地文本。 |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | 获取 PivotTable 中 "(All)" 标签的文本。 |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | 获取 "All Periods" 的本地化文本。 |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | 获取 PivotTable 中 "Column Labels" 标签的文本。 |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | 获取 PivotTable 中值区域字段标题的文本。 |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | 获取 "Days" 的本地文本。 |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | 获取 PivotTable 中 "(blank)" 标签的文本。 |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | 获取 PivotTable 中 "Grand Total" 标签的文本。 |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | 获取 "Hours" 的本地文本。 |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | 获取 "Minutes" 的本地文本。 |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | 获取 "Months" 的本地文本。 |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | 获取 PivotTable 中 "(Multiple Items)" 标签的文本。 |
| virtual [GetTextOfOr](../../aspose.cells.settings/pivotglobalizationsettings/gettextofor/)() | 获取 "or" 的所有本地格式化字符串。 |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | 获取指定受保护名称的文本。 |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**已废弃。**) 获取 PivotTable 中的保护名称。 |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | 获取 "Quarters" 的本地文本。 |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | 获取 "Range" 的本地文本 |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | 获取 PivotTable 中 "Row Labels" 标签的文本。 |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | 获取 "Seconds" 的本地文本 |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | 获取 PivotTable 中 [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) 类型的文本。 |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | 获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法。 |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | 获取 "Years" 的本地文本。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGlobalizationSettingsDemo
    {
        public static void PivotGlobalizationSettingsExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["B5"].PutValue(250);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 创建 PivotGlobalizationSettings 的实例
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // 演示各种方法的使用
            Console.WriteLine("Text of Total: " + globalizationSettings.GetTextOfTotal());
            Console.WriteLine("Text of Grand Total: " + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine("Text of Multiple Items: " + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
            Console.WriteLine("Text of Protection: " + globalizationSettings.GetTextOfProtection());
            Console.WriteLine("Text of Column Labels: " + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine("Text of Row Labels: " + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine("Text of Empty Data: " + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine("Text of Data Field Header: " + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine("Text of Years: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Text of Quarters: " + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
            Console.WriteLine("Text of Days: " + globalizationSettings.GetTextOfDays());
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

            // GetTextOfProtectedName 方法示例
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // GetTextOfSubTotal 方法示例
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // 保存工作簿
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


