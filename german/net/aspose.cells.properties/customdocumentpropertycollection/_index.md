---
title: "Klasse CustomDocumentPropertyCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.CustomDocumentPropertyCollection Klasse. Eine Sammlung benutzerdefinierter Dokumenteigenschaften"
type: docs
url: /de/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

Eine Sammlung benutzerdefinierter Dokumenteigenschaften.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Gibt ein [`DocumentProperty`](../documentproperty/) Objekt nach Index zurück. (Vererbt von [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Gibt ein [`DocumentProperty`](../documentproperty/)-Objekt anhand des Namens der Eigenschaft zurück. (Vererbt von [`DocumentPropertyCollection`](../documentpropertycollection/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Boolean**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.DateTime**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Float**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Number**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.String**. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert. (Vererbt von [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Liest den Index einer Eigenschaft anhand ihres Namens. (Vererbt von [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung. (Vererbt von [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Entfernt eine Eigenschaft am angegebenen Index. (2 Methoden) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind (Verwenden Sie den Zellenwert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind (Verwenden Sie den Wert der benutzerdefinierten Dokumenteigenschaft, um den Zellenwert des verknüpften Bereichs zu aktualisieren). |

### Hinweise

Jedes [`DocumentProperty`](../documentproperty/)‑Objekt stellt eine benutzerdefinierte Eigenschaft eines Containerdokuments dar.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomDocumentPropertyCollectionDemo
    {
        public static void CustomDocumentPropertyCollectionExample()
        {
            // Instanziiere ein Workbook-Objekt
            Workbook workbook = new Workbook();

            // Rufe eine Liste aller benutzerdefinierten Dokumenteigenschaften der Excel-Datei ab.
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Benutzerdefinierte Dokumenteigenschaften hinzufügen
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Eine verknüpfte benutzerdefinierte Dokumenteigenschaft hinzufügen
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Verknüpfte Eigenschaftswerte aktualisieren
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Zugriff auf benutzerdefinierte Dokumenteigenschaften
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Benutzerdefinierte Dokumenteigenschaften ausgeben
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
    }
}
```

### Siehe auch

* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


