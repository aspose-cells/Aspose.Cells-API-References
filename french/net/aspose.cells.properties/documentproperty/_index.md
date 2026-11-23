---
title: "Classe DocumentProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Properties.DocumentProperty class. Représente une propriété de document personnalisée ou intégrée"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Représente une propriété de document personnalisée ou intégrée.

```csharp
public class DocumentProperty
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Renvoie true si cette propriété n'a pas de nom dans le stockage OLE2 et qu'un nom unique a été généré uniquement pour l'API publique. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indique si cette propriété est liée au contenu |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Renvoie le nom de la propriété. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | La source de contenu liée. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Obtient le type de données de la propriété. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Obtient ou définit la valeur de la propriété. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Renvoie la valeur de la propriété en tant que bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Renvoie la valeur de la propriété en tant que DateTime dans le fuseau horaire local. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Renvoie la valeur de la propriété en tant que double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Renvoie la valeur de la propriété en tant qu'entier. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Renvoie la valeur de la propriété en tant que chaîne. |

### Exemples

```csharp

[C#]

//Instanciez un objet Workbook
Workbook workbook = new Workbook("book1.xls");
 
//Récupérer une liste de toutes les propriétés personnalisées du document Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Accéder à une propriété personnalisée en utilisant l'indice de la propriété
DocumentProperty customProperty1 = customProperties[3];
 
//Accéder à une propriété personnalisée en utilisant le nom de la propriété
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

### Voir aussi

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


