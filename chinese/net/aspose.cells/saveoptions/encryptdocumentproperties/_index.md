---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SaveOptions 属性。指示在保存为 .xls 文件时是否加密文档属性。默认值为 true"
type: docs
url: /zh/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### 备注

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // 创建示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置一些文档属性
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // 设置密码保护
            workbook.Settings.Password = "password123";
            
            // 保存时将 EncryptDocumentProperties = true（默认）
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // 保存时将 EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // 通过重新加载进行验证
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### 另请参见

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


