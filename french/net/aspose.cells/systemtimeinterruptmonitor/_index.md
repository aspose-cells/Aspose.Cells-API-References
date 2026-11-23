---
title: "Classe SystemTimeInterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.SystemTimeInterruptMonitor. Implémentation simple de AbstractInterruptMonitor en vérifiant et comparant l'heure système actuelle avec la limite spécifiée par l'utilisateur"
type: docs
url: /fr/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Implémentation simple de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) en vérifiant et comparant l'heure système actuelle avec la limite spécifiée par l'utilisateur.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Construit un moniteur d'interruption. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Cette implémentation vérifie simplement si le temps écoulé (du moment où le moniteur a démarré jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Voir [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Démarre le moniteur avec la limite de temps spécifiée. L'heure de départ pour calculer le temps écoulé est simplement le moment où cette méthode est appelée, ainsi la procédure à surveiller doit être lancée immédiatement après cet appel. |

### Remarques

Cette implémentation est simplement une solution basique pour des scénarios simples. Elle doit récupérer et vérifier fréquemment l'heure système, ce qui peut avoir un impact négatif sur les performances dans une certaine mesure.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Créer une instance de SystemTimeInterruptMonitor avec terminateWithoutException défini sur false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Créer LoadOptions et définir InterruptMonitor sur le moniteur créé
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Commencer la surveillance avec une limite de temps de 1000 millisecondes (1 seconde)
            monitor.StartMonitor(1000);

            try
            {
                // Charger un classeur avec les LoadOptions spécifiés
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Si le temps de chargement du fichier modèle dépasse une seconde, une interruption sera requise et une exception sera levée ici
                // Sinon, commencez à surveiller la procédure d'enregistrement avec une nouvelle limite de temps
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Enregistrez le classeur
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


