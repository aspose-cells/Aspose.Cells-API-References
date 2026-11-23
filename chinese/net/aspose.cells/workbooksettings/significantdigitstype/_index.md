---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取和设置此工作簿中输出数值时的有效数字类型。默认值为 SignificantDigitsType"
type: docs
url: /zh/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

获取和设置此工作簿中输出数值时的有效数字类型。默认值为 [`SignificantDigitsType`](../../cellshelper/significantdigitstype/)。

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问 WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // 显示当前 SignificantDigitsType 值
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // 演示设置不同的 SignificantDigitsType 值
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // 添加一些数值数据以演示效果
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // 保存工作簿
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### 另请参见

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


