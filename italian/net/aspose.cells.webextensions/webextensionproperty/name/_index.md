---
title: "WebExtensionProperty.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionProperty. Ottiene e imposta un nome di proprietà personalizzato"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Ottiene e imposta il nome di una proprietà personalizzata.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Imposta e dimostra la proprietà Name
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Modifica e visualizza il nome aggiornato
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


