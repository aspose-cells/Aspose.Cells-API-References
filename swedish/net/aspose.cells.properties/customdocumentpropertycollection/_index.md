---
title: CustomDocumentPropertyCollection
second_title: Aspose.Cells för .NET API-referens
description: En samling anpassade dokumentegenskaper.
type: docs
weight: 4830
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

En samling anpassade dokumentegenskaper.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.properties/documentpropertycollection/count) { get; } | Får antal föremål i samlingen. |
| [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Returnerar en[`DocumentProperty`](../documentproperty)objekt efter index. |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Returnerar en[`DocumentProperty`](../documentproperty) objekt efter egenskapens namn. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add)(string, bool) | Skapar en ny anpassad dokumentegenskap för **PropertyType.Boolean** datatyp. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_3)(string, DateTime) | Skapar en ny anpassad dokumentegenskap för **PropertyType.DateTime** datatyp. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_1)(string, double) | Skapar en ny anpassad dokumentegenskap för **PropertyType.Float** datatyp. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_2)(string, int) | Skapar en ny anpassad dokumentegenskap för **PropertyType.Number** datatyp. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_4)(string, string) | Skapar en ny anpassad dokumentegenskap för **PropertyType.String** datatyp. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent)(string, string) | Skapar en ny anpassad dokumentegenskap som länkar till innehåll. |
| [Clear](../../aspose.cells.properties/documentpropertycollection/clear)() | Tar bort alla egenskaper från samlingen. |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains)(string) | Returnerar sant om en egenskap med det angivna namnet finns i samlingen. |
| [GetEnumerator](../../aspose.cells.properties/documentpropertycollection/getenumerator)() |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof)(string) | Hämtar indexet för en egenskap efter namn. |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove)(string) | Tar bort en egenskap med det angivna namnet från samlingen. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat)(int) | Tar bort en egenskap vid det angivna indexet. |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue)() | Uppdatera anpassat dokumentegenskapsvärde som länkar till innehåll. |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange)() | Uppdatera anpassad dokumentegenskapsvärde till länkat intervall. |

### Anmärkningar

Varje[`DocumentProperty`](../documentproperty) objekt representerar en anpassad egenskap för ett containerdokument.

### Exempel

```csharp

[C#]

//Instantiera ett arbetsboksobjekt
Workbook workbook = new Workbook("book1.xls");

//Hämta en lista över alla anpassade dokumentegenskaper för Excel-filen
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As New Workbook("book1.xls")

'Hämta en lista över alla anpassade dokumentegenskaper för Excel-filen
Dim customProperties As CustomDocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties

```

### Se även

* class [DocumentPropertyCollection](../documentpropertycollection)
* namnutrymme [Aspose.Cells.Properties](../../aspose.cells.properties)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->