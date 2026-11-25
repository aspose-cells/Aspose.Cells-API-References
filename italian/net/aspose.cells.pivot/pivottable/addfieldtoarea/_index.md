---
title: "PivotTable.AddFieldToArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Aggiunge il campo all'area specifica"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Aggiunge il campo all'area specifica.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | Il tipo di area dei campi. |
| fieldName | String | Il nome nei campi base. |

### Valore di ritorno

La posizione del campo nei campi specifici. Se non esiste un campo con quel nome, restituisce -1.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 2000;
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 1200;

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Aggiungi campi a diverse aree usando AddFieldToArea con nomi di campo stringa
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Region");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna e calcola la tabella pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Aggiunge il campo all'area specifica.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | Il tipo di area dei campi. |
| baseFieldIndex | Int32 | L'indice nei campi di base. |

### Valore di ritorno

La posizione del campo nei campi specifici.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il PivotTable
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
                worksheet.Cells["C" + i].PutValue(i * 100);
            }

            // Aggiungi una PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Aggiungi campi alle aree usando AddFieldToArea(PivotFieldType, Int32)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Aggiunge il campo all'area specifica.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | il tipo di area dei campi. |
| pivotField | PivotField | il campo nei campi base. |

### Valore di ritorno

la posizione del campo nei campi specifici.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro con dati di origine
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "Source Data";
            
            // Aggiungi dati di esempio
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Region");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Product A");
            sourceSheet.Cells["B2"].PutValue("North");
            sourceSheet.Cells["C2"].PutValue(1000);
            
            sourceSheet.Cells["A3"].PutValue("Product B");
            sourceSheet.Cells["B3"].PutValue("South");
            sourceSheet.Cells["C3"].PutValue(2000);
            
            sourceSheet.Cells["A4"].PutValue("Product A");
            sourceSheet.Cells["B4"].PutValue("East");
            sourceSheet.Cells["C4"].PutValue(1500);
            
            sourceSheet.Cells["A5"].PutValue("Product B");
            sourceSheet.Cells["B5"].PutValue("West");
            sourceSheet.Cells["C5"].PutValue(2500);

            // Aggiungi una tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = "='Source Data'!A1:C5";
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            // Aggiungi campi alle aree
            pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
            
            // Aggiungi campo dati
            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            // Aggiungi campo dati all'area colonna usando il parametro PivotField
            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


