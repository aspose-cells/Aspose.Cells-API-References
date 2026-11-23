---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Retourne une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Retourne une collection [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document intégrées de la feuille de calcul.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Remarques

Une nouvelle propriété ne peut pas être ajoutée à la liste des propriétés de document intégrées. Vous ne pouvez que récupérer une propriété intégrée et modifier sa valeur. La liste suivante présente les noms des propriétés intégrées :

Titre

Sujet

Auteur

Mots-clés

Commentaires

Modèle

Dernier auteur

Numéro de révision

Nom de l'application

Date de la dernière impression

Date de création

Heure du dernier enregistrement

Temps total d'édition

Nombre de pages

Nombre de mots

Nombre de caractères

Sécurité

Catégorie

Format

Gestionnaire

Entreprise

Nombre d'octets

Nombre de lignes

Nombre de paragraphes

Nombre de diapositives

Nombre de notes

Nombre de diapositives masquées

Nombre de clips multimédias

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


