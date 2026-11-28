---
title: "Class CellsFactory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsFactory sınıfı. Cells modelinin sınıflarını örneklemek için yardımcı araç"
type: docs
url: /tr/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Cells modelinin sınıflarını örneklemek için araç.

```csharp
public class CellsFactory
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Yeni bir stil oluşturur. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // CellsFactory'nin yeni bir örneğini oluşturun
            CellsFactory factory = new CellsFactory();

            // Fabrikayı kullanarak yeni bir Stil oluşturun
            Style style = factory.CreateStyle();

            // Stili özelleştirin
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Yeni bir çalışma kitabı ve çalışma sayfası oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Stili belirli bir hücreye uygulayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


