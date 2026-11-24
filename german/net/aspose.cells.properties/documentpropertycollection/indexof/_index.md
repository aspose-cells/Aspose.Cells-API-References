---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentPropertyCollection‑Methode. Gibt den Index einer Eigenschaft anhand ihres Namens zurück."
type: docs
url: /de/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Ermittelt den Index einer Eigenschaft anhand des Namens.

```csharp
public int IndexOf(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Groß-/Kleinschreibung‑unabhängige Name der Eigenschaft. |

### Rückgabewert

Der nullbasierte Index. Negativer Wert, wenn nicht gefunden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Die Sammlung integrierter Dokumenteigenschaften abrufen
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Für integrierte Eigenschaften können wir nur Werte vorhandener Eigenschaften setzen
            // Um benutzerdefinierte Eigenschaften hinzuzufügen, müssten wir CustomDocumentPropertyCollection verwenden
            // Hier setzen wir nur einige vorhandene integrierte Eigenschaften zur Demonstration
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Rufen Sie die IndexOf‑Methode mit einem Zeichenkettenparameter auf
                int index = properties.IndexOf("Subject");
                
                // Ergebnis anzeigen
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Zeige die Eigenschaft am gefundenen Index
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


