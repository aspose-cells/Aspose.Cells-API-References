---
title: "Workbook.CreateStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Crea un nuovo stile"
type: docs
url: /it/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Crea un nuovo stile.

```csharp
public Style CreateStyle()
```

### Valore di ritorno

Restituisce un oggetto stile.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un nuovo stile usando il metodo CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // Imposta le proprietà dello stile
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Crea il flag di stile e imposta i flag
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Applica lo stile alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Adatta automaticamente la colonna
            worksheet.AutoFitColumn(0);
            
            // Salva la cartella di lavoro
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Crea un nuovo stile.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cloneDefaultStyle | Booleano | Indica se clona lo stile predefinito |

### Valore di ritorno

Restituisce un oggetto stile.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Crea un nuovo stile (false = non ereditare dallo stile predefinito)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Applica lo stile a una cella
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Salva la cartella di lavoro
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


