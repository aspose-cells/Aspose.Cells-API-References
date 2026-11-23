---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "OdsSaveOptions 属性。获取和设置 ODF 版本"
type: docs
url: /zh/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

获取和设置 ODF 版本。

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // 创建 ODS 保存选项
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // 将 ODF 版本设置为 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // 使用指定的 ODF 版本保存
            workbook.Save("OdfVersion12.ods", saveOptions);

            // 更改为 ODF 版本 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### 另请参见

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


