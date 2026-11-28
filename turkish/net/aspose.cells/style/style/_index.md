---
title: "Style.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yapıcı. Style sınıfının yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells/style/style/
---
## Style constructor

[`Style`](../) sınıfının yeni bir örneğini başlatır.

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Açıklamalar

NOT: Bu yapıcı artık kullanımdan kaldırıldı. Bunun yerine lütfen CellsFactory.CreateStyle() yöntemini kullanın. Bu özellik Ekim 2016'dan itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yapıcıyı kullanarak bir stil oluşturun
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


