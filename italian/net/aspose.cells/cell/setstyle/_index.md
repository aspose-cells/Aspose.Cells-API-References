---
title: "Cell.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta lo stile della cella"
type: docs
url: /it/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Imposta lo stile della cella.

```csharp
public void SetStyle(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | Lo stile della cella. |

### Osservazioni

Se le impostazioni del bordo vengono modificate, il bordo delle celle di regolazione verrà aggiornato anch'esso.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile e imposta le sue proprietà
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Applica lo stile alla cella B2 (1,1 nell'indice a base zero)
            cells[1, 1].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Applica la proprietà modificata dello stile alla cella.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | Lo stile della cella. |
| explicitFlag | Booleano | True, sovrascrive solo la formattazione che è impostata esplicitamente. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea gli stili direttamente
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // Applica gli stili alle celle con il metodo SetStyle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Salva la cartella di lavoro
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Applica lo stile della cella in base ai flag.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | Lo stile della cella. |
| flag | StyleFlag | Il flag di stile. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea uno stile e imposta le sue proprietà
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Crea un flag di stile e impostalo per applicare tutta la formattazione
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Recupera le celle e imposta il valore su A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Applica lo stile alla cella usando SetStyle
            cell.SetStyle(style, flag);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


