---
title: "Klasse WebExtensionBinding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionBinding Klasse. Stellt eine Bindungsbeziehung zwischen einem Office-Add-In und den Daten im Dokument dar"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Stellt eine Bindungsbeziehung zwischen einem Office-Add-In und den Daten im Dokument dar.

```csharp
public class WebExtensionBinding
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Liefert und setzt den Bindungsschlüssel, der verwendet wird, um den Bindungseintrag in dieser Liste mit den gebundenen Daten im Dokument zu verknüpfen. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Liefert und setzt den Bindungsbezeichner. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Liest und setzt den Bindungstyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine neue WebExtensionBinding-Instanz
                WebExtensionBinding binding = new WebExtensionBinding();

                // Eigenschaften festlegen
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Eigenschaftswerte anzeigen
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Eigenschaften ändern
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


