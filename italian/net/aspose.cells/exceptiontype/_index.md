---
title: "Enum ExceptionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ExceptionType. Rappresenta il codice del tipo di eccezione personalizzato"
type: docs
url: /it/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Rappresenta il codice del tipo di eccezione personalizzata.

```csharp
public enum ExceptionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Chart | `0` | Impostazione del grafico non valida. |
| DataType | `1` | Impostazione del tipo di dato non valida. |
| DataValidation | `2` | Impostazione di convalida dei dati non valida. |
| ConditionalFormatting | `3` | Impostazione di convalida dei dati non valida. |
| FileFormat | `4` | Formato file non valido. |
| Formula | `5` | Formula non valida. |
| InvalidData | `6` | Dati non validi. |
| InvalidOperator | `7` | Operatore non valido. |
| IncorrectPassword | `8` | Password errata. |
| License | `9` | Errori relativi alla licenza. |
| Limitation | `10` | Errore di superamento dei limiti di MS Excel. |
| PageSetup | `11` | Impostazione di configurazione pagina non valida. |
| PivotTable | `12` | Impostazione della tabella pivot non valida. |
| Shape | `13` | Impostazione dell'oggetto di disegno non valida. |
| Sparkline | `14` | Impostazione dell'oggetto sparkline non valida. |
| SheetName | `15` | Nome del foglio di lavoro non valido. |
| SheetType | `16` | Tipo di foglio di lavoro non valido. |
| Interrupted | `17` | Il processo è interrotto. |
| IO | `18` | Il file non è valido. |
| Permission | `19` | È necessaria l'autorizzazione per aprire questo file. |
| UnsupportedFeature | `20` | Funzionalità non supportata. |
| UnsupportedStream | `21` | Flusso non supportato da aprire. |
| UndisclosedInformation | `22` | I file contengono alcune informazioni non divulgate. |
| FileCorrupted | `23` | Il contenuto del file è corrotto. |
| DefinedName | `25` | Nome definito non valido |
| Font | `26` | Carattere non valido |
| AutoFilter | `27` | Impostazione del filtro automatico non valida. |
| FontSubstitution | `28` | Tipo di avviso di sostituzione del carattere quando un carattere non è stato trovato; questo tipo di avviso può essere ottenuto. |

### Esempi

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
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();

                // Tentativo di impostare un nome di foglio di lavoro non valido per generare un'eccezione
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Salva la cartella di lavoro
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Gestire l'eccezione CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Verifica il tipo di eccezione
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Aggiungi altri casi secondo necessità per diversi tipi di eccezione
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Gestisci eventuali altre eccezioni
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


