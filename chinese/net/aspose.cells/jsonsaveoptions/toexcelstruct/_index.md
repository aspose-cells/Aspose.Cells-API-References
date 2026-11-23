---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。指示是否将 Excel 文件转换为 JSON 结构"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

指示是否将 Excel 文件转换为 JSON 结构。

```csharp
public bool ToExcelStruct { get; set; }
```

### 备注

仅用于将范围转换为 JSON。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向单元格添加示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // 创建要导出的范围
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // 使用 ToExcelStruct 配置 JSON 保存选项
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // 将范围导出为 JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


