---
title: "Metered.GetProductName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Metered 方法。获取产品名称"
type: docs
url: /zh/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

获取产品名称

```csharp
public string GetProductName()
```

### 返回值

产品名称

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // 创建计量实例
            Metered metered = new Metered();
            
            // 设置计量密钥（替换为实际密钥）
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // 获取并显示产品名称
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // 演示使用简单电子表格的基本用法
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


