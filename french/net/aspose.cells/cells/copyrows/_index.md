---
title: "Cells.CopyRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Copie les données et les formats de certaines lignes complètes"
type: docs
url: /fr/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copie les données et les formats de certaines lignes entières.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | Int32 | Indice de ligne source. |
| destinationRowIndex | Int32 | Indice de ligne de destination. |
| rowNumber | Int32 | Le numéro de la ligne copiée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Ajoutez quelques données d'exemple au classeur source
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Obtenez les cellules des deux classeurs
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Copiez toutes les lignes de la source vers la destination en commençant à la ligne 0 dans la destination
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Enregistrer le résultat
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copie les données et les formats de certaines lignes entières.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | Int32 | Indice de ligne source. |
| destinationRowIndex | Int32 | Indice de ligne de destination. |
| rowNumber | Int32 | Le numéro de la ligne copiée. |
| copyOptions | CopyOptions | Les options de copie. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez quelques données d'exemple et des hyperliens
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Insérez une ligne vide à la ligne 5
            worksheet.Cells.InsertRows(5, 1);

            // Copier la ligne 4 vers la ligne 5 sans CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Réinitialiser la feuille de calcul
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Insérer à nouveau une ligne vide à la ligne 5
            worksheet.Cells.InsertRows(5, 1);

            // Copier la ligne 4 vers la ligne 5 avec CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copie les données et les formats de certaines lignes entières.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceRowIndex | Int32 | Indice de ligne source. |
| destinationRowIndex | Int32 | Indice de ligne de destination. |
| rowNumber | Int32 | Le numéro de la ligne copiée. |
| copyOptions | CopyOptions | Les options de copie. |
| pasteOptions | PasteOptions | les options de collage. |

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


