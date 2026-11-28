---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionTaskPane özelliği. Görev bölmesinin UI'da belgeye kilitlenip kilitlenmediğini ve kullanıcının kapatıp kapatamayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Görev bölmesinin UI'da belgeye kilitlenip kilitlenmediğini ve kullanıcının kapatıp kapatamayacağını gösterir.

```csharp
public bool IsLocked { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // Çalışma kitabının web uzantısı koleksiyonu aracılığıyla görev bölmesi oluştur
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


