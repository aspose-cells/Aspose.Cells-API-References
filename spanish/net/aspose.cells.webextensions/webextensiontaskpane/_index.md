---
title: "Clase WebExtensionTaskPane"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionTaskPane. Representa un objeto de panel de tareas persistente"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Representa un objeto de panel de tareas persistente.

```csharp
public class WebExtensionTaskPane
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Obtiene y establece la última ubicación acoplada de este objeto de panel de tareas. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Indica si el panel de tareas está bloqueado al documento en la interfaz de usuario y no puede ser cerrado por el usuario. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Indica si el Panel de tareas se muestra visible por defecto cuando se abre el documento. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Obtiene y establece el índice, enumerando de fuera a dentro, de este panel de tareas entre otros paneles de tareas persistentes acoplados en la misma ubicación predeterminada. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Obtiene y establece la parte de extensión web asociada con la instancia del panel de tareas. |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Obtiene y establece el valor de ancho predeterminado para esta instancia del panel de tareas. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


