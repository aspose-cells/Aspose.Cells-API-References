---
title: "Classe PivotPageFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotPageFields. Rappresenta gli elementi di pagina della pivot se la fonte dati della tabella pivot è un intervallo di consolidamento. Può contenere al massimo 4 elementi."
type: docs
url: /it/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Rappresenta gli elementi di pagina pivot se l'origine dati della tabella pivot è costituita da intervalli di consolidamento. Può contenere al massimo 4 elementi.

```csharp
public class PivotPageFields
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Rappresenta gli elementi del campo di pagina della pivot. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Ottiene il numero di campi di pagina. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Imposta quale etichetta dell'elemento in ogni campo di pagina utilizzare per identificare l'intervallo dati. La lunghezza di pageItemIndex deve essere uguale a PageFieldCount, quindi aggiungi prima il campo di pagina. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Aggiunge un campo di pagina. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotPageFieldsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Sheet1";
            FillData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            FillData(sheet2);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;

            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields pageFields = new PivotPageFields();

            pageFields.AddPageField(new string[] { "item1", "item2" });
            pageFields.AddPageField(new string[] { "item3", "item4" });

            pageFields.AddIdentify(0, new int[] { 0, 1 });
            pageFields.AddIdentify(1, new int[] { 1, -1 });

            pivotTables.Add(src, false, pageFields, "E3", "PivotTable1");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }

        private static void FillData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Value");
            cells["C1"].PutValue("Date");

            for (int i = 1; i < 8; i++)
            {
                cells[$"A{i+1}"].PutValue($"Item{i}");
                cells[$"B{i+1}"].PutValue(i * 100);
                cells[$"C{i+1}"].PutValue(System.DateTime.Now.AddDays(i).ToString("yyyy-MM-dd"));
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


