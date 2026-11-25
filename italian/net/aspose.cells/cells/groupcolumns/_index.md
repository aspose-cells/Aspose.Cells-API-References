---
title: "Cells.GroupColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Raggruppa le colonne"
type: docs
url: /it/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Raggruppa le colonne.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima colonna da raggruppare. |
| lastIndex | Int32 | L'indice dell'ultima colonna da raggruppare. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Raggruppa le colonne dall'indice 0 al 255
            cells.GroupColumns(0, 255);

            // Salva la cartella di lavoro
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Raggruppa le colonne.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima colonna da raggruppare. |
| lastIndex | Int32 | L'indice dell'ultima colonna da raggruppare. |
| isHidden | Booleano | Specifica se le colonne raggruppate sono nascoste. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Raggruppa le colonne da 5 a 7 (3 colonne) e nascondile.
            cells.GroupColumns(5, 7, true);

            // Salva la cartella di lavoro
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


