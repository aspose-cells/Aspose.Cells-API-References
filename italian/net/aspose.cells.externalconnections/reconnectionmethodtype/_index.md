---
title: "Enum ReConnectionMethodType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType enum. Specifica cosa deve fare l'applicazione di foglio di calcolo quando una connessione fallisce"
type: docs
url: /it/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Specifica cosa deve fare l'applicazione di foglio di calcolo quando una connessione fallisce.

```csharp
public enum ReConnectionMethodType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Required | `1` | All'aggiornamento utilizza le informazioni di connessione esistenti e, se risultano non valide, ottiene le informazioni di connessione aggiornate, se disponibili dal file di connessione esterno. |
| Always | `2` | Ad ogni aggiornamento ottieni le informazioni di connessione aggiornate dal file di connessione esterno, se disponibili, e usale al posto delle informazioni di connessione esistenti. In questo caso l'aggiornamento dei dati fallirà se il file di connessione esterno non è disponibile. |
| Never | `3` | Non ottenere mai informazioni di connessione aggiornate dal file di connessione esterno anche se è disponibile e anche se le informazioni di connessione esistenti sono non valide |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Dimostrare la creazione e l'uso dei valori enum ReConnectionMethodType
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Mostrare l'uso in un'istruzione switch
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


