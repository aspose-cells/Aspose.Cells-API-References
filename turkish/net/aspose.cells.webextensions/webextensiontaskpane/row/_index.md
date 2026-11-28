---
title: "WebExtensionTaskPane.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionTaskPane özelliği. Aynı varsayılan konumda yerleştirilmiş diğer kalıcı görev bölmeleri arasında bu görev bölmesinin dıştan içe doğru sayılan indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Bu görev bölmesinin, aynı varsayılan konumda yer alan diğer kalıcı görev bölmeleri arasında dıştan içe doğru numaralandırılan dizinini alır ve ayarlar.

```csharp
public int Row { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir web uzantısı ekle
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Web uzantısı özelliklerini yapılandır
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Bir görev bölmesi ekle
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Görev bölmesi özelliklerini yapılandır
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Row özelliğinin kullanımını göster
            taskPane.Row = 5; // Set row position
            
            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


