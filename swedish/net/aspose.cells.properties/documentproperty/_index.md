---
title: "Klass DocumentProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.DocumentProperty-klass. Representerar en anpassad eller inbyggd dokumentegenskap"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Representerar en anpassad eller inbyggd dokumentegenskap.

```csharp
public class DocumentProperty
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Returnerar true om denna egenskap inte har ett namn i OLE2-lagringen och ett unikt namn genererades endast för det offentliga API:et. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indikerar om denna egenskap är länkad till innehåll |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Returnerar egenskapens namn. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | Den länkade innehållskällan. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Hämtar datatypen för egenskapen. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Hämtar eller anger värdet för egenskapen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Returnerar egenskapsvärdet som bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Returnerar egenskapsvärdet som DateTime i lokal tidszon. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Returnerar egenskapsvärdet som double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Returnerar egenskapsvärdet som integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Returnerar egenskapsvärdet som en sträng. |

### Exempel

```csharp

[C#]

//Instansiera ett Workbook-objekt
Workbook workbook = new Workbook("book1.xls");
 
//Hämta en lista över alla anpassade dokumentegenskaper i Excel-filen
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Åtkomst till en anpassad dokumentegenskap genom att använda egenskapsindexet
DocumentProperty customProperty1 = customProperties[3];
 
//Åtkomst till en anpassad dokumentegenskap genom att använda egenskapsnamnet
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Instantiate a Workbook object
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Retrieve a list of all custom document properties of the Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Accessng a custom document property by using the property index
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Accessng a custom document property by using the property name
Dim customProperty2 As DocumentProperty = customProperties("Owner")
```

### Se även

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


