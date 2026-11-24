---
title: "Klasse DocumentProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.DocumentProperty‑Klasse. Stellt eine benutzerdefinierte oder integrierte Dokumenteigenschaft dar."
type: docs
url: /de/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Stellt eine benutzerdefinierte oder integrierte Dokumenteigenschaft dar.

```csharp
public class DocumentProperty
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Gibt true zurück, wenn diese Eigenschaft keinen Namen im OLE2‑Speicher hat und ein eindeutiger Name ausschließlich für die öffentliche API erzeugt wurde. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Gibt an, ob diese Eigenschaft mit Inhalt verknüpft ist. |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Gibt den Namen der Eigenschaft zurück. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | Die verknüpfte Inhaltsquelle. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Ermittelt den Datentyp der Eigenschaft. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Ermittelt oder setzt den Wert der Eigenschaft. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Gibt den Eigenschaftswert als bool zurück. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Gibt den Eigenschaftswert als DateTime in der lokalen Zeitzone zurück. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Gibt den Eigenschaftswert als double zurück. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Gibt den Eigenschaftswert als integer zurück. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Gibt den Eigenschaftswert als Zeichenkette zurück. |

### Beispiele

```csharp

[C#]

//Instanziiere ein Workbook-Objekt
Workbook workbook = new Workbook("book1.xls");
 
//Rufe eine Liste aller benutzerdefinierten Dokumenteigenschaften der Excel-Datei ab.
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Zugriff auf eine benutzerdefinierte Dokumenteigenschaft über den Eigenschaftsindex.
DocumentProperty customProperty1 = customProperties[3];
 
//Zugriff auf eine benutzerdefinierte Dokumenteigenschaft über den Eigenschaftsnamen.
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

### Siehe auch

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


