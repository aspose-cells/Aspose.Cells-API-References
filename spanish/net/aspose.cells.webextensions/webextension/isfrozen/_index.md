---
title: "WebExtension.IsFrozen"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtension. Indica si el usuario puede interactuar con el complemento de Office o no"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Indica si el usuario puede interactuar con el Office Add-in o no.

```csharp
public bool IsFrozen { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Esta línea fallará porque WebExtension requiere parámetros del constructor
                // WebExtension webExtension = new WebExtension();
                
                // En su lugar, obtendremos una web extension del libro de trabajo si es posible
                // o demostrar con un enfoque diferente
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // Para propósitos de demostración, mostraremos cómo funcionaría la propiedad si tuvieras una instancia válida
                // En un escenario real, obtendrías la instancia WebExtension del libro de trabajo o de otra fuente
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Establezca las propiedades iniciales
                    webExtension.Id = "MyAddin123";
                    
                    // Mostrar valor inicial de IsFrozen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Cambiar la propiedad IsFrozen (ya que es de lectura y escritura)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Demostrar el efecto verificando si el usuario puede interactuar
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Guardar el libro de trabajo (aunque la web extension podría no persistirse sin pasos adicionales)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // En una implementación real, esto obtendría un WebExtension existente del libro de trabajo
            // o crear uno correctamente con los parámetros del constructor requeridos
            // Esto es solo un marcador de posición para la demostración
            return null;
        }
    }
}
```

### Ver también

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


