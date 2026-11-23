---
title: "Classe AbstractInterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AbstractInterruptMonitor. Moniteur des demandes d'interruption dans toutes les opérations longues"
type: docs
url: /fr/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Surveille les demandes d'interruption dans toutes les opérations gourmandes en temps.

```csharp
public abstract class AbstractInterruptMonitor
```

## Propriétés

| Nom | Description |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Indique si une interruption est demandée pour l'opération en cours. Si true, alors l'opération en cours sera interrompue. L'implémentation doit effectuer ici une vérification rapide et efficace, sinon cela peut devenir un autre goulot d'étranglement pour la procédure. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Lorsque la procédure est interrompue, qu'elle termine la procédure silencieusement ou lève une Exception. La valeur par défaut est false, c'est-à-dire, lorsque [`IsInterruptionRequested`](./isinterruptionrequested/) est true, une [`CellsException`](../cellsexception/) avec le code Interrupted sera levée. |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Implémentation personnalisée de AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //le fichier de résultat est correct
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Logique pour déterminer si une interruption est demandée
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// le fichier de résultat plante
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("Obtenir la valeur de retour indiquant s'il faut interrompre le programme===");
        //        // Logique pour déterminer si une interruption est demandée
        //        //return false; // Modifiez ceci en fonction de votre logique
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Modifiez ceci en fonction de votre logique
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Créez une instance de CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Définissez les options de chargement avec le moniteur d'interruption personnalisé
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Chargez le classeur avec les options spécifiées
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Effectuez les calculs
            workbook.CalculateFormula();

            // Enregistrez le classeur
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


