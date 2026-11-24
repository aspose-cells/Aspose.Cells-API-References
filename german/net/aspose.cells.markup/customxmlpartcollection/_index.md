---
title: "Klasse CustomXmlPartCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.CustomXmlPartCollection Klasse. Stellt einen Custom XML Data Storage Part innerhalb eines Pakets dar."
type: docs
url: /de/net/aspose.cells.markup/customxmlpartcollection/
---
## CustomXmlPartCollection class

Stellt einen benutzerdefinierten XML‑Datenspeicherteil dar (benutzerdefinierte XML‑Daten innerhalb eines Pakets).

```csharp
public class CustomXmlPartCollection : CollectionBase<CustomXmlPart>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/customxmlpartcollection/item/) { get; } | Liefert ein Element am angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.markup/customxmlpartcollection/add/)(byte[], byte[]) | Fügt ein Element zur Sammlung hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomXmlPart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomXmlPart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SelectByID](../../aspose.cells.markup/customxmlpartcollection/selectbyid/)(string) | Liefert ein Element nach ID. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassCustomXmlPartCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Hole die CustomXmlPartCollection aus der Arbeitsmappe
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;

            // Erstelle Beispiel-XML-Daten und -Schema
            byte[] xmlData = System.Text.Encoding.UTF8.GetBytes("<root><item>Test</item></root>");
            byte[] schemaData = System.Text.Encoding.UTF8.GetBytes("<xsd:schema xmlns:xsd='http://www.w3.org/2001/XMLSchema'></xsd:schema>");

            // Füge einen neuen benutzerdefinierten XML-Teil hinzu
            int index = customXmlParts.Add(xmlData, schemaData);

            // Hole den hinzugefügten XML-Teil nach Index
            CustomXmlPart part = customXmlParts[index];

            // Wähle XML-Teil nach ID aus (falls bekannt)
            string partId = part.ID;
            CustomXmlPart selectedPart = customXmlParts.SelectByID(partId);

            // Füge einen weiteren XML-Teil hinzu
            byte[] xmlData2 = System.Text.Encoding.UTF8.GetBytes("<data><value>123</value></data>");
            customXmlParts.Add(xmlData2, null);

            // Zeige die Anzahl der benutzerdefinierten XML-Teile an.
            Console.WriteLine("Custom XML parts count: " + customXmlParts.Count);

            // Speichere die Arbeitsmappe
            workbook.Save("CustomXmlPartCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomXmlPart](../customxmlpart/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


