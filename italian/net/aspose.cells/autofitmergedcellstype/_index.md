---
title: "Enum AutoFitMergedCellsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.AutoFitMergedCellsType. Rappresenta il tipo di adattamento automatico delle celle unite"
type: docs
url: /it/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Rappresenta il tipo di adattamento automatico delle celle unite.

```csharp
public enum AutoFitMergedCellsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Ignora le celle unite. |
| FirstLine | `1` | Espande solo l'altezza della prima riga. |
| LastLine | `2` | Espande solo l'altezza dell'ultima riga. |
| EachLine | `3` | Espande l'altezza di ogni riga. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            //Ottenere il riferimento del foglio di lavoro appena aggiunto
            Worksheet sheet1 = workbook.Worksheets[0];

            // Creare un intervallo A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Unisci le celle
            range.Merge();

            // Inserire un valore nella cella unita A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Crea un oggetto stile
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Attivare l'andare a capo del testo
            style.IsTextWrapped = true;

            // Applica lo stile alla cella
            sheet1.Cells[0, 0].SetStyle(style);

            // Creare un oggetto per AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // Espande solo l'altezza della prima riga.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Adattare automaticamente le righe nel foglio (incluse le celle unite)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Creare un intervallo A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Unisci le celle
            range2.Merge();

            // Inserire un valore nella cella unita A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Crea un oggetto stile
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Attivare l'andare a capo del testo
            style2.IsTextWrapped = true;

            // Applica lo stile alla cella
            sheet2.Cells[0, 0].SetStyle(style);

            // Creare un oggetto per AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Espande solo l'altezza dell'ultima riga.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Adattare automaticamente le righe nel foglio (incluse le celle unite)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Creare un intervallo A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Unisci le celle
            range3.Merge();

            // Inserire un valore nella cella unita A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Crea un oggetto stile
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Attivare l'andare a capo del testo
            style3.IsTextWrapped = true;

            // Applica lo stile alla cella
            sheet3.Cells[0, 0].SetStyle(style);

            // Creare un oggetto per AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Espande solo l'altezza di ogni riga.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Adattare automaticamente le righe nel foglio (incluse le celle unite)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Creare un intervallo A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Unisci le celle
            range4.Merge();

            // Inserire un valore nella cella unita A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Crea un oggetto stile
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Attivare l'andare a capo del testo
            style4.IsTextWrapped = true;

            // Applica lo stile alla cella
            sheet4.Cells[0, 0].SetStyle(style);

            // Creare un oggetto per AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Ignora le celle unite.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Adattare automaticamente le righe nel foglio (escluse le celle unite)
            sheet4.AutoFitRows(options4);

            // Salva la cartella di lavoro
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


