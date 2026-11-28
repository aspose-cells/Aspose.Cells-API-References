---
title: "CellsHelper.GetUsedColors"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Çalışma kitabındaki kullanılan tüm renkleri alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Çalışma kitabında kullanılan tüm renkleri alır.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çalışma kitabı | Çalışma Kitabı | Çalışma kitabı nesnesi. |

### Dönüş Değeri

Kullanılan renkler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kullanılan renkleri göstermek için bazı renkli hücreler ekleyin
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // GetUsedColors yöntemini çalışma kitabı parametresiyle çağırın
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Kullanılan renkleri gösterin
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


