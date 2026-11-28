---
title: "Sınıf PaneCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PaneCollection sınıfı. Belirtilen pencerede gösterilen tüm Pane nesnelerini temsil eder"
type: docs
url: /tr/net/aspose.cells/panecollection/
---
## PaneCollection class

Belirtilen pencerede gösterilen tüm Pane nesnelerini temsil eder.

```csharp
public class PaneCollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) Etkin bölmeyi alır ve ayarlar. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Etkin bölmeyi alır ve ayarlar. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Sağ bölmenin ilk görünen sütununu alır ve ayarlar. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Alt bölmenin ilk görünen satırını alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Satır 5, sütun 1'de bölmeleri dondur
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Bölme koleksiyonunu al
            PaneCollection panes = sheet.GetPanes();
            
            // Bölme ayarlarını değiştir
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


