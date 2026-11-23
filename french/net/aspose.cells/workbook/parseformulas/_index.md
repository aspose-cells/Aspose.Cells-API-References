---
title: "Workbook.ParseFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis un fichier modèle ou affectées à une cellule"
type: docs
url: /fr/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis le fichier modèle ou affectées à une cellule.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Indique s'il faut ignorer les erreurs pour une formule invalide. Pour une formule invalide, si l'erreur est ignorée, cette formule sera ignorée et le processus continuera à analyser les autres formules, sinon une exception sera levée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les formules sans analyse (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Analyser toutes les formules d'un coup
            wb.ParseFormulas(false);

            // Vérifier les formules
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


