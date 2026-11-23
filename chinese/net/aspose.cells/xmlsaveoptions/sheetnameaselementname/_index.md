---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlSaveOptions 属性。指示是否将工作表名称导出为元素的名称"
type: docs
url: /zh/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

指示是否将工作表的名称导出为元素的名称。

```csharp
public bool SheetNameAsElementName { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // 创建包含数据的示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // 使用 SheetNameAsElementName = true（默认）保存
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // 使用 SheetNameAsElementName = false 保存
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### 另请参见

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


