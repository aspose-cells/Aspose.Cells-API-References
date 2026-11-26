---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfBookmarkEntry. Cuando esta propiedad es verdadera, la entrada de marcador se colapsará; de lo contrario, se expandirá"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Cuando esta propiedad es verdadera, la bookmarkentry se colapsará, de lo contrario se expandirá.

```csharp
public bool IsCollapse { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyIsCollapseDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Crear entrada de marcador raíz
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Crear una sección financiera colapsada
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Agregar subsecciones trimestrales a la sección financiera
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Crear una sección operativa expandida
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Construir la jerarquía de marcadores
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Asignar marcadores a las opciones de guardado
            saveOptions.Bookmark = rootEntry;

            // Guardar con los marcadores configurados
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Ver también

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


