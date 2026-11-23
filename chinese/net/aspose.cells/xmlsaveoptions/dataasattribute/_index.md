---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlSaveOptions 属性。指示是否将数据导出为元素的属性"
type: docs
url: /zh/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

指示是否将数据导出为元素的属性。

```csharp
public bool DataAsAttribute { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // 创建 XML 保存选项，并将 DataAsAttribute 设置为 true
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // 将数据保存为属性
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // 更改为将数据保存为元素
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### 另请参见

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


