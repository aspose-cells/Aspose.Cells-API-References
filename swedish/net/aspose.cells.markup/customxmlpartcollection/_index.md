---
title: "Klass CustomXmlPartCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.CustomXmlPartCollection-klass. Representerar en Custom XML Data Storage Part med anpassad XML-data inom ett paket"
type: docs
url: /sv/net/aspose.cells.markup/customxmlpartcollection/
---
## CustomXmlPartCollection class

Representerar en anpassad XML‑databasdel (anpassad XML‑data inom ett paket).

```csharp
public class CustomXmlPartCollection : CollectionBase<CustomXmlPart>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/customxmlpartcollection/item/) { get; } | Hämtar ett objekt på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.markup/customxmlpartcollection/add/)(byte[], byte[]) | Lägger till ett objekt i samlingen. |
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
| [SelectByID](../../aspose.cells.markup/customxmlpartcollection/selectbyid/)(string) | Hämtar ett objekt efter id. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta CustomXmlPartCollection från arbetsboken
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;

            // Skapa exempel på XML-data och schema
            byte[] xmlData = System.Text.Encoding.UTF8.GetBytes("<root><item>Test</item></root>");
            byte[] schemaData = System.Text.Encoding.UTF8.GetBytes("<xsd:schema xmlns:xsd='http://www.w3.org/2001/XMLSchema'></xsd:schema>");

            // Lägg till en ny anpassad XML-del
            int index = customXmlParts.Add(xmlData, schemaData);

            // Hämta den tillagda XML-delen efter index
            CustomXmlPart part = customXmlParts[index];

            // Välj XML-del efter ID (om känt)
            string partId = part.ID;
            CustomXmlPart selectedPart = customXmlParts.SelectByID(partId);

            // Lägg till ytterligare en XML-del
            byte[] xmlData2 = System.Text.Encoding.UTF8.GetBytes("<data><value>123</value></data>");
            customXmlParts.Add(xmlData2, null);

            // Visa antalet anpassade XML-delar
            Console.WriteLine("Custom XML parts count: " + customXmlParts.Count);

            // Spara arbetsboken
            workbook.Save("CustomXmlPartCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomXmlPart](../customxmlpart/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


