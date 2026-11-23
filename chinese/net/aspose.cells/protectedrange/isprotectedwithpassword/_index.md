---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ProtectedRange 属性。指示工作表是否受密码保护"
type: docs
url: /zh/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

指示工作表是否受密码保护。

```csharp
public bool IsProtectedWithPassword { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建受保护的范围并获取其索引
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // 保护工作表以强制执行限制
            worksheet.Protect(ProtectionType.All);
            
            // 验证密码保护状态
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### 另请参见

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


