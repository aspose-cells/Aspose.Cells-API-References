---
title: "WorkbookSettings.Region"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta le impostazioni regionali per il foglio di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Ottiene o imposta le impostazioni regionali per il workbook.

```csharp
public CountryCode Region { get; set; }
```

### Osservazioni

1. Impostazioni regionali utilizzate dal componente Aspose.Cells per una cartella di lavoro caricata da un file modello: i). Per un file XLS, esistono campi definiti per le impostazioni regionali e MS Excel salva i dati delle impostazioni regionali nel file durante il salvataggio del file XLS. Pertanto, utilizziamo la regione salvata nel file modello per la cartella di lavoro. Se non si desidera utilizzare la regione salvata nel file XLS, si prega di reimpostarla su quella prevista (ad esempio, CountryCode.Default) dopo aver caricato il file modello. Inoltre, salviamo anche il valore specificato dall'utente (tramite questo metodo) nel file durante il salvataggio di un file XLS. ii). Per altri formati di file, come XLSX, XLSB... ecc., non è definito alcun campo per le impostazioni regionali nella specifica del formato file. Pertanto, utilizziamo le impostazioni regionali dell'ambiente dell'applicazione per la cartella di lavoro. E il valore specificato dall'utente (tramite questo metodo) non può essere mantenuto per i file generati con tali formati. 2. Per l'effetto di visualizzazione in MS Excel: le impostazioni regionali applicate qui possono avere effetto solo a runtime con il componente Aspose.Cells e non durante la visualizzazione del file generato con MS Excel. Anche per il file XLS generato in cui i dati delle impostazioni regionali specificate sono stati salvati, quando lo si visualizza/modifica con MS Excel, la regione utilizzata da MS Excel per eseguire la formattazione è sempre quella predefinita dell'ambiente in cui MS Excel è in esecuzione, non quella salvata nel file. È un comportamento di MS Excel e non può essere modificato tramite codice.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Vedi anche

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


