---
title: "ImportTableOptions.Styles"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImportTableOptions 属性。获取并设置表中每列的样式"
type: docs
url: /zh/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

获取并设置表中每列的样式。

```csharp
public Style[] Styles { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建示例数据表
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // 创建 ImportTableOptions 并设置 Styles 属性
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // 为每列创建样式
                Style[] columnStyles = new Style[2];

                // Product 列的样式（粗体，蓝色字体）
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Price 列的样式（货币格式，绿色字体）
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // 设置 Styles 属性
                options.Styles = columnStyles;

                // 导入带样式的数据
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // 显示已应用的样式
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // 保存工作簿
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


