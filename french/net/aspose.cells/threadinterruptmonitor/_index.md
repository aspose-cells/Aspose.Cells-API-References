---
title: "Classe ThreadInterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ThreadInterruptMonitor. Implémentation simple de AbstractInterruptMonitor en démarrant un autre thread pour demander l'interruption après une temporisation de la limite spécifiée par l'utilisateur"
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Implémentation simple de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) en démarrant un autre thread pour demander l'interruption après une temporisation de la limite spécifiée par l'utilisateur.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Construit un moniteur d'interruption. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Cette implémentation vérifie simplement si le temps écoulé (du moment où le moniteur a démarré jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Voir [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Termine le moniteur pour une procédure. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Démarre le moniteur avec la limite de temps spécifiée. L'heure de départ pour calculer le temps écoulé est simplement le moment où cette méthode est appelée, ainsi la procédure à surveiller doit être lancée immédiatement après cet appel. |

### Remarques

Une instance de moniteur peut être utilisée de manière répétée, tant que vous surveillez chaque processus séquentiellement. Elle ne doit pas être utilisée pour surveiller plusieurs procédures simultanément dans des multithreads.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Créez une instance de ThreadInterruptMonitor avec terminateWithoutException défini sur false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Créer LoadOptions et définir InterruptMonitor sur le moniteur créé
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Démarrez le moniteur avec une limite de temps de 1000 millisecondes (1 seconde)
            monitor.StartMonitor(1000);

            try
            {
                // Charger un classeur avec les LoadOptions spécifiés
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Terminez le moniteur pour la procédure de chargement
                monitor.FinishMonitor();

                // Redémarrez le moniteur avec une nouvelle limite de temps de 1500 millisecondes (1,5 seconde)
                monitor.StartMonitor(1500);

                // Enregistrez le classeur
                wb.Save("result.xlsx");

                // Terminez le moniteur pour la procédure d'enregistrement
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


