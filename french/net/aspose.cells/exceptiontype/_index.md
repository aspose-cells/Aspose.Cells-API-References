---
title: "Énumération ExceptionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.ExceptionType. Représente le code de type d'exception personnalisé"
type: docs
url: /fr/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Représente le code du type d'exception personnalisé.

```csharp
public enum ExceptionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Chart | `0` | Paramètre de graphique invalide. |
| DataType | `1` | Paramètre de type de données invalide. |
| DataValidation | `2` | Paramètre de validation de données invalide. |
| ConditionalFormatting | `3` | Paramètre de validation de données invalide. |
| FileFormat | `4` | Format de fichier invalide. |
| Formula | `5` | Formule invalide. |
| InvalidData | `6` | Données invalides. |
| InvalidOperator | `7` | Opérateur invalide. |
| IncorrectPassword | `8` | Mot de passe incorrect. |
| License | `9` | Erreurs liées à la licence. |
| Limitation | `10` | Erreur de dépassement des limites de MS Excel. |
| PageSetup | `11` | Paramètre de mise en page invalide. |
| PivotTable | `12` | Paramètre de tableau croisé dynamique invalide. |
| Shape | `13` | Paramètre d'objet de dessin invalide. |
| Sparkline | `14` | Paramètre d'objet de sparkline invalide. |
| SheetName | `15` | Nom de feuille de calcul invalide. |
| SheetType | `16` | Type de feuille de calcul invalide. |
| Interrupted | `17` | Le processus est interrompu. |
| IO | `18` | Le fichier est invalide. |
| Permission | `19` | Une autorisation est requise pour ouvrir ce fichier. |
| UnsupportedFeature | `20` | Fonctionnalité non prise en charge. |
| UnsupportedStream | `21` | Flux non pris en charge à ouvrir. |
| UndisclosedInformation | `22` | Les fichiers contiennent des informations non divulguées. |
| FileCorrupted | `23` | Le contenu du fichier est corrompu. |
| DefinedName | `25` | Nom défini invalide |
| Font | `26` | Police invalide |
| AutoFilter | `27` | Paramètre de filtre automatique invalide. |
| FontSubstitution | `28` | Type d'avertissement de substitution de police lorsqu'une police n'a pas été trouvée, ce type d'avertissement peut être obtenu. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();

                // Tentative de définir un nom de feuille de calcul invalide pour déclencher une exception
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Enregistrez le classeur
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Gérer l'exception CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Vérifiez le type d'exception
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Ajoutez plus de cas si nécessaire pour différents types d'exception
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Gérez toutes les autres exceptions
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


