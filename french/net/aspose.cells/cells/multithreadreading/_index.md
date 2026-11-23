---
title: "Cells.MultiThreadReading"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture MultiThread. La valeur par défaut de cette propriété est false"
type: docs
url: /fr/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. La valeur par défaut de cette propriété est false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Remarques

Si plusieurs threads lisent des objets Row/Cell dans cette collection de manière concurrente, cette propriété doit être définie sur true, sinon des résultats inattendus peuvent être produits. Prendre en charge la lecture Multi-Thread peut dégrader les performances lors de l'accès aux objets Row/Cell de cette collection. Veuillez noter que certaines fonctionnalités ne peuvent pas prendre en charge la lecture Multi-Thread, comme le formatage des valeurs (par [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), etc.). Ainsi, même si cette propriété est définie sur true, ces API peuvent toujours donner des résultats inattendus lors de la lecture Multi-Thread.

### Exemples

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Activer la lecture multi-thread
            cells.MultiThreadReading = true;

            // Configurer le style pour la première colonne
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Remplir les cellules avec des données d'exemple
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Créer des threads pour lire les valeurs des cellules
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // Attendre que tous les threads soient terminés
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


