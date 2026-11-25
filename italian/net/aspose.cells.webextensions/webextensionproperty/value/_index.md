---
title: "WebExtensionProperty.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionProperty. Ottiene e imposta un valore di proprietà personalizzato"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Ottiene e imposta il valore di una proprietà personalizzata.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Imposta e dimostra la proprietà Value
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Modifica e mostra il valore aggiornato
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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


