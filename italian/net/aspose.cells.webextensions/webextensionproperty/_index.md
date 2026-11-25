---
title: "Classe WebExtensionProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionProperty. Rappresenta una proprietà personalizzata di un Office Addin"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Rappresenta una proprietà personalizzata di Office Add-in.

```csharp
public class WebExtensionProperty
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Ottiene e imposta il nome di una proprietà personalizzata. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Ottiene e imposta il valore di una proprietà personalizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Imposta i valori delle proprietà
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Visualizza i valori delle proprietà
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


