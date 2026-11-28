---
title: "HtmlSaveOptions.SheetSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır (Visible)."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Birden fazla çalışma sayfasına sahip yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Gösterim amacıyla bir sayfayı gizli yapın
            workbook.Worksheets[1].IsVisible = false;

            // Her sayfada bazı örnek veriler ayarlayın
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // HtmlSaveOptions örneği oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Mevcut SheetSet değerini göster (varsayılan null'dur, bu da tüm görünür sayfalar anlamına gelir)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // SheetSet'i yalnızca belirli sayfaları (indeksle) içerecek şekilde ayarlayın
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // HTML olarak kaydedin - yalnızca belirtilen sayfalar dahil edilecektir
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // SheetSet'i yalnızca görünür sayfalara değiştirin
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // SheetSet'i yalnızca etkin sayfaya değiştirin
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


