---
title: "ActiveXControlBase.Data"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Kontrolün ikili verisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Kontrolün ikili verilerini alır ve ayarlar.

```csharp
public virtual byte[] Data { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.Drawing;

    public class ActiveXControlBasePropertyDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = "MyList";
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = ("A3:A7");
            list.Value = ("Apple");
            list.LinkedCell = ("A1");
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);

            // İlk Data özelliği bilgilerini göster
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Data'yı etkileyen kontrol özelliklerini değiştir
            list.BackOleColor = 0xFF0000;

            // Güncellenmiş Data özelliği bilgilerini göster
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Değişikliklerin kalıcı olduğunu göstermek için çalışma kitabını kaydet
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


