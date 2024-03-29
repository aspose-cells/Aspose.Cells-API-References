---
title: DocumentProperty
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente une propriété de document personnalisée ou intégrée.
type: docs
weight: 4860
url: /fr/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Représente une propriété de document personnalisée ou intégrée.

```csharp
public class DocumentProperty
```

## Propriétés

| Nom | La description |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname) { get; } | Renvoie vrai si cette propriété n'a pas de nom dans le stockage OLE2 et qu'un nom unique a été généré uniquement pour l'API publique. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent) { get; } | Indique si cette propriété est liée à content |
| [Name](../../aspose.cells.properties/documentproperty/name) { get; } | Renvoie le nom de la propriété. |
| [Source](../../aspose.cells.properties/documentproperty/source) { get; } | La source de contenu liée. |
| [Type](../../aspose.cells.properties/documentproperty/type) { get; } | Obtient le type de données de la propriété. |
| [Value](../../aspose.cells.properties/documentproperty/value) { get; set; } | Obtient ou définit la valeur de la propriété. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool)() | Renvoie la valeur de la propriété sous la forme bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime)() | Renvoie la valeur de la propriété sous la forme DateTime dans le fuseau horaire local. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble)() | Renvoie la valeur de la propriété sous la forme double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint)() | Renvoie la valeur de la propriété sous forme d'entier. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring)() | Renvoie la valeur de la propriété sous forme de chaîne. |

### Exemples

```csharp

[C#]

//Instancier un objet Workbook
Workbook workbook = new Workbook("book1.xls");
 
//Récupérer une liste de toutes les propriétés de document personnalisées du fichier Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
// Accéder à une propriété de document personnalisée à l'aide de l'index de propriété
DocumentProperty customProperty1 = customProperties[3];
 
// Accéder à une propriété de document personnalisée en utilisant le nom de la propriété
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Instancier un objet Workbook
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Récupérer une liste de toutes les propriétés de document personnalisées du fichier Excel
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Accéder à une propriété de document personnalisée à l'aide de l'index de propriété
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Accéder à une propriété de document personnalisée à l'aide du nom de la propriété
Dim customProperty2 As DocumentProperty = customProperties("Owner")
```

### Voir également

* espace de noms [Aspose.Cells.Properties](../../aspose.cells.properties)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
