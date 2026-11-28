---
title: "Sınıf WebExtensionTaskPane"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionTaskPane sınıfı. Kalıcı bir görev bölmesi nesnesini temsil eder."
type: docs
url: /tr/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Kalıcı bir görev bölmesi nesnesinin temsilidir.

```csharp
public class WebExtensionTaskPane
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Bu görev bölmesi nesnesinin son bağlandığı konumu alır ve ayarlar. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Görev bölmesinin UI'da belgeye kilitlenip kilitlenmediğini ve kullanıcının kapatıp kapatamayacağını gösterir. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Belge açıldığında Görev Bölmesinin varsayılan olarak görünür olup olmadığını gösterir. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Bu görev bölmesinin, aynı varsayılan konumda yer alan diğer kalıcı görev bölmeleri arasında dıştan içe doğru numaralandırılan dizinini alır ve ayarlar. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Görev bölmesi örneğiyle ilişkili web uzantısı bölümünü alır ve ayarlar. |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Bu görev bölmesi örneği için varsayılan genişlik değerini alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionTaskPaneDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


