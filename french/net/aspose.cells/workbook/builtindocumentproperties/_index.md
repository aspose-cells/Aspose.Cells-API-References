---
title: "Workbook.BuiltInDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Retourne une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

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
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder et modifier les propriétés de document intégrées
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // Afficher les propriétés modifiées
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


