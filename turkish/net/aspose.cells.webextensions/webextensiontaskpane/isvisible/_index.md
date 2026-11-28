---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionTaskPane özelliği. Belge açıldığında Görev Bölmesi'nin varsayılan olarak görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Belge açıldığında Görev Bölmesinin varsayılan olarak görünür olup olmadığını gösterir.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir web uzantısı ekle
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Web uzantısı özelliklerini yapılandır
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Bir görev bölmesi ekle
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Görev bölmesi özelliklerini yapılandır
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // IsVisible özelliğini göster
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


