---
title: "AbstractLowCodeProtectionProvider.GetWorksheetProtectionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeProtectionProvider 方法。获取用于保护指定工作表的保护类型"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

获取用于保护指定工作表的保护类型。

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### 返回值

用于保护指定工作表的保护类型。None 表示工作表不受保护。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("newSheet");
            string name = worksheet.Name;
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
               
                // 显示结果
                Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorksheetProtectionType(string sheetName)
            {
                return ProtectionType.Structure;
            }

            public override string GetWorksheetPassword(string sheetName)
            {
                return $"aspose123_{sheetName}";
            }
        }

    }
    
}
```

### 另请参见

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


