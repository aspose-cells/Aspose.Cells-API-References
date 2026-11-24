---
title: "WebExtensionPropertyCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionPropertyCollection-Eigenschaft. Gibt die Eigenschaft der WebExtension anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Gibt die Eigenschaft der WebExtension anhand des Index zurück.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die Eigenschaft der WebExtension.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine WebExtension-Eigenschaftssammlung
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Einige Eigenschaften hinzufügen
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Zugriff auf Eigenschaften über den Item‑Indexer
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Eigenschaftswerte über die Sammlung ändern
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Die Änderungen demonstrieren
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Arbeitsmappe speichern (obwohl Web-Extension-Eigenschaften im gespeicherten Dokument ohne entsprechende Einrichtung nicht sichtbar sind)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Liest die Eigenschaft der Web-Extension.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name der Eigenschaft. |

### Rückgabewert

Die Eigenschaft der WebExtension.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine WebExtension-Eigenschaftssammlung
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Füge Eigenschaften zur Sammlung hinzu
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Zugriff auf Eigenschaften über den Item-Indexer
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Eigenschaftswerte ändern (Hinweis: Item ist schreibgeschützt, daher müssen wir Add/Remove verwenden)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Aktualisierten Wert anzeigen
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


