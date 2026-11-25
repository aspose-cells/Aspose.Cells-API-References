---
title: "Classe DocumentProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Properties.DocumentProperty class. Rappresenta una proprietà del documento personalizzata o incorporata"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Rappresenta una proprietà del documento personalizzata o integrata.

```csharp
public class DocumentProperty
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Restituisce true se questa proprietà non ha un nome nello storage OLE2 ed è stato generato un nome univoco solo per l'API pubblica. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indica se questa proprietà è collegata al contenuto |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Restituisce il nome della proprietà. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | L'origine del contenuto collegato. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Ottiene il tipo di dati della proprietà. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Ottiene o imposta il valore della proprietà. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Restituisce il valore della proprietà come bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Restituisce il valore della proprietà come DateTime nel fuso orario locale. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Restituisce il valore della proprietà come double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Restituisce il valore della proprietà come integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Restituisce il valore della proprietà come stringa. |

### Esempi

```csharp

[C#]

//Istanzia un oggetto Workbook
Workbook workbook = new Workbook("book1.xls");
 
//Recupera un elenco di tutte le proprietà personalizzate del documento Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Accesso a una proprietà del documento personalizzata usando l'indice della proprietà
DocumentProperty customProperty1 = customProperties[3];
 
//Accesso a una proprietà del documento personalizzata usando il nome della proprietà
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

### Vedi anche

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


