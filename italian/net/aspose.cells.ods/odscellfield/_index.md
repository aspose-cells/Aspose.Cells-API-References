---
title: "Classe OdsCellField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Ods.OdsCellField. Rappresenta il campo cella di ods"
type: docs
url: /it/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Rappresenta il campo cella di ODS.

```csharp
public class OdsCellField
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Ottiene e imposta l'indice di colonna della cella. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Rappresenta il formato personalizzato del valore del campo. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Ottiene e imposta il tipo del campo. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Ottiene e imposta l'indice di riga della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Crea un OdsCellField tramite la collezione (senza costruttore senza parametri)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Recupera il campo appena aggiunto
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Scrivi qualcosa nella cella identificata da OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Aggiungi nuovamente lo stesso campo per dimostrare l'uso della collezione (opzionale)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Aggiorna tutti i campi ODS affinché siano riflessi nel file salvato
                odsFields.UpdateFieldsValue();

                // Visualizza i valori delle proprietà nella console
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Salva la cartella di lavoro come file ODS
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


