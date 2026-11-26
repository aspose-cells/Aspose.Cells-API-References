---
title: "WebExtension.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtension. Obtiene y establece el identificador único de la instancia del complemento de Office en el documento actual"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Obtiene y establece la identificación única de la instancia del Office Add-in en el documento actual.

```csharp
public string Id { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenga la colección de extensiones web del libro de trabajo
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Agregue una nueva extensión web (esto la creará con los parámetros requeridos)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Establezca la propiedad Id (ya que es de lectura-escritura)
                webExtension.Id = "SampleAddin123";
                
                // Muestre el valor actual de la propiedad Id
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Modifique la propiedad Id para demostrar que es editable
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Guarda el libro de trabajo
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


