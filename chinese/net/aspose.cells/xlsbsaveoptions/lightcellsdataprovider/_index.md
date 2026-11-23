---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XlsbSaveOptions 属性。用于在轻模式下保存工作簿的数据提供程序"
type: docs
url: /zh/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

用于在轻模式下保存工作簿的数据提供程序。

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充一些示例数据
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // 创建 XLSB 保存选项
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // 使用 LightCellsDataProvider 保存工作簿
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // 验证已保存的数据
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // 在此实现单元格迭代逻辑
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // 在此实现行迭代逻辑
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // 在此实现单元格处理逻辑
        }

        public void StartRow(Row row)
        {
            // 在此实现行处理逻辑
        }

        public bool StartSheet(int sheetIndex)
        {
            // 在此实现工作表处理逻辑
            return true; // Return true to process the sheet
        }
    }
}
```

### 另请参见

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


