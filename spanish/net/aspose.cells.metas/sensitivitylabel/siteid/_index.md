---
title: "SensitivityLabel.SiteId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Representa el identificador del sitio de Azure Active Directory (Azure AD) correspondiente a la política de etiqueta de sensibilidad que describe la etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Representa el identificador del sitio de Azure Active Directory (Azure AD) correspondiente a la política de etiqueta de sensibilidad que describe la etiqueta de sensibilidad.

```csharp
public string SiteId { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Crear una instancia de etiqueta de sensibilidad
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));

                // Establecer propiedades básicas
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;

                // Demuestre la obtención del valor inicial de SiteId
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Establezca SiteId a un identificador de sitio Azure AD de ejemplo
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Cambie SiteId para demostrar que es de lectura y escritura
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Muestre cómo SiteId se relaciona con otras propiedades
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Guarda el libro de trabajo
                workbook.Save("SiteIdDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


