---
title: "Enum DateTimeGroupingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DateTimeGroupingType enum. Specifica come raggruppare i valori dateTime"
type: docs
url: /it/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Specifica come raggruppare i valori dateTime.

```csharp
public enum DateTimeGroupingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Day | `0` | Raggruppa per giorno. |
| Hour | `1` | Raggruppa per ora. |
| Minute | `2` | Raggruppa per minuto. |
| Month | `3` | Raggruppa per mese. |
| Second | `4` | Raggruppa per secondo. |
| Year | `5` | Raggruppa per anno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Creazione di una cartella di lavoro e accesso al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Creazione di un AutoFilter e impostazione dell'intervallo
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Aggiunta di filtri di data con diversi DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Salvataggio della cartella di lavoro
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


