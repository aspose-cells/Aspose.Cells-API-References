---
title: "Clase WebExtensionReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionReference. Representa la identificación de la ubicación del proveedor y la versión de la extensión"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Representa la identificación de la ubicación del proveedor y la versión de la extensión.

```csharp
public class WebExtensionReference
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Obtiene y establece el identificador asociado con el complemento de Office dentro de un proveedor de catálogo. El identificador DEBE ser único dentro de un proveedor de catálogo. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Obtiene y establece la instancia del marketplace donde se almacena el complemento de Office. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Obtiene y establece el tipo de marketplace que identifica el atributo de almacén. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Obtiene y establece la versión. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Cree primero una WebExtension
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Obtenga la WebExtensionReference de la WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Establezca las propiedades de la WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Muestre las propiedades de referencia
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Guarda el libro de trabajo
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


