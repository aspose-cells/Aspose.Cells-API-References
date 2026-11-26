---
title: "WebExtension.AlterReferences"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtension. Obtiene una lista de referencias alternativas"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Obtiene una lista de alter references.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenga la colección de extensiones web del libro de trabajo
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Agregar una nueva extensión web
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Acceda a la propiedad AlterReferences (solo lectura)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Mostrar información sobre las referencias alter
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Agregar una nueva referencia alter (demuestra el uso de la colección)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Mostrar recuento actualizado
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Guarda el libro de trabajo
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


