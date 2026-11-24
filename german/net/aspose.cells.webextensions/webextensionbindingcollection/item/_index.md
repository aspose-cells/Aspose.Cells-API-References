---
title: "WebExtensionBindingCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionBindingCollection-Eigenschaft. Gibt die Web-Extension-Bindungsbeziehung anhand des angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Liest die WebExtension-Bindungsbeziehung anhand des angegebenen Index.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die Web-Extension-Bindungsbeziehung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Web-Extension-Bindungssammlung
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Füge der Sammlung eine neue Bindung hinzu
            int index = bindingCollection.Add();

            // Greife auf die Bindung über die Item-Eigenschaft zu (schreibgeschützt)
            WebExtensionBinding binding = bindingCollection[index];

            // Setze Eigenschaften der Bindung
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Zeige die Details der Bindung an
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Ändere die Bindung über die Sammlung
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


