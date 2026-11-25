---
title: "Classe CellsHelper"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellsHelper. Fornisce funzioni di supporto"
type: docs
url: /it/net/aspose.cells/cellshelper/
---
## CellsHelper class

Fornisce funzioni di supporto.

```csharp
public class CellsHelper
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Ottiene o imposta il percorso di avvio alternativo, a cui si fa riferimento da alcune formule esterne. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Ottiene o imposta la factory per creare istanze con implementazione speciale. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Ottiene i DPI della macchina. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc. |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Ottiene o imposta il percorso della libreria a cui si fa riferimento da alcune formule esterne. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Ottiene e imposta il numero di cifre significative. Il valore predefinito è 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Ottiene e imposta il tipo predefinito di cifre significative per l'emissione di valori numerici. Il valore predefinito è G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Ottiene o imposta il percorso di avvio a cui si fa riferimento da alcune formule esterne. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Aggiungi la funzione add-in. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Ottiene gli indici di riga e colonna della cella in base al suo nome. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Ottiene l'indice della colonna in base al nome della colonna. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsoleto.**) Converte la formula A1 della cella nella formula r1c1. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsoleto.**) Converte la formula r1c1 della cella nella formula A1. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con ' ', quindi verrà restituito il valore della stringa ricostruita. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con il carattere fornito, quindi verrà restituito il valore della stringa ricostruita. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Converte il valore double in valore data/ora. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Converte la data/ora in valore double. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Ottiene la larghezza del testo in unità di punti. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Ottiene tutti i colori utilizzati nella cartella di lavoro. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Ottiene la versione di rilascio. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Unisce alcuni file xls di grandi dimensioni in un file xls. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Indica se il nome del foglio deve essere racchiuso tra virgolette singole. |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Ottiene il nome della riga in base all'indice della riga. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Ottiene l'indice della riga in base al nome della riga. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Imposta la cartella per i file temporanei che possono essere usati come cache dei dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Impostazione delle proprietà di CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Supponendo che CustomImplementationFactory sia già definito e istanziato altrove
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Dimostrazione dell'uso delle proprietà di CellsHelper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Esempio di utilizzo di CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


