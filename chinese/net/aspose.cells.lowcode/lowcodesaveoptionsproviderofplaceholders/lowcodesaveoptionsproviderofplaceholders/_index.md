---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfPlaceHolders 构造函数。实例化一个对象，以根据指定的模板提供保存选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

实例化一个对象，根据指定的模板提供保存选项。

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pathTemplate | String | 生成的文件路径的模板。 |

### 备注

文件路径模板中支持的占位符：${SheetIndex}：将被拆分部分的工作表索引替换${SheetName}：将被拆分部分的工作表名称替换${SplitPartIndex}：将被拆分部分的索引替换${SheetIndexPrefix}：将被[`SheetIndexPrefix`](../sheetindexprefix/) 替换${SheetNamePrefix}：将被[`SheetNamePrefix`](../sheetnameprefix/) 替换${SplitPartPrefix}：将被[`SplitPartPrefix`](../splitpartprefix/) 替换

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 使用 String 参数调用 #ctor 方法
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // 设置一些属性
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


