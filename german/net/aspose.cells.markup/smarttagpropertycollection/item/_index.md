---
title: "SmartTagPropertyCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagPropertyCollection-Eigenschaft. Gibt ein SmartTagProperty-Objekt zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Gibt ein [`SmartTagProperty`](../../smarttagproperty/) Objekt zurück.

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Rückgabewert

Gibt ein [`SmartTagProperty`](../../smarttagproperty/) Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Smart‑Tag‑Eigenschaftssammlung
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Füge Eigenschaften zur Sammlung hinzu
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Zugriff auf Eigenschaften über den Item‑Indexer
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Zeige aktuelle Eigenschaftswerte an
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Hinweis: Die Item‑Eigenschaft ist schreibgeschützt, sodass wir ihr nicht direkt einen Wert zuweisen können
            // Stattdessen können wir die Eigenschaften der zurückgegebenen SmartTagProperty‑Objekte ändern
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Zeige aktualisierte Werte an
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Speichere die Arbeitsmappe (obwohl Smart‑Tags bei einem einfachen Speichern nicht sichtbar gespeichert werden)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Gibt ein [`SmartTagProperty`](../../smarttagproperty/) Objekt anhand des Namens der Eigenschaft zurück.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name der Eigenschaft. |

### Rückgabewert

Gibt ein [`SmartTagProperty`](../../smarttagproperty/) Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Smart‑Tag‑Einstellung und füge ein Smart‑Tag hinzu
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Rufe das Smart‑Tag und seine Eigenschaften ab
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Füge einige Eigenschaften hinzu, um die Item‑Eigenschaft zu demonstrieren
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Greife auf Eigenschaften über den Item‑Indexer zu (nach Index)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Zeige die Eigenschaftswerte an
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Speichere die Arbeitsmappe
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


