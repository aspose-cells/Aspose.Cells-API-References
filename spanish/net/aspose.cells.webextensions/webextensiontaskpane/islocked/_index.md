---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Indica si el panel de tareas está bloqueado al documento en la interfaz de usuario y no puede ser cerrado por el usuario"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Indica si el panel de tareas está bloqueado al documento en la interfaz de usuario y no puede ser cerrado por el usuario.

```csharp
public bool IsLocked { get; set; }
```

### Ejemplos

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
                // Crear un panel de tareas a través de la colección de extensiones web del libro de trabajo
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

### Ver también

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


