---
title: WorkbookRender classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 130
url: /fr/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender classe
 Représente un rendu de classeur.
Le constructeur de cette classe , doit être utilisé après modification de pagesetup, style cellule.



Le type WorkbookRender expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | La construction de WorkbookRender|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [page_count](/cells/fr/python-net/aspose.cells.rendering/workbookrender/page_count) | Obtient le nombre total de pages des classeurs.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [to_image(stream)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Rendre le classeur entier en tant qu'image Tiff à diffuser.|
| [to_image(filename)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Rendre le classeur entier en tant qu'image Tiff dans un fichier.|
| [to_image(page_index, file_name)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Afficher certaines pages dans un fichier.|
| [to_image(page_index, stream)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Afficher certaines pages dans un flux.|
| [to_printer(printer_name)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Rendre le classeur à l'imprimante|
| [to_printer(printer_name, job_name)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Rendre le classeur à l'imprimante|
| [to_printer(printer_settings)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Rendre le classeur à l'imprimante|
| [to_printer(printer_settings, job_name)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Rendre le classeur à l'imprimante|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Rendre le classeur à l'imprimante|
| [get_page_size_inch(page_index)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |Obtenez la taille de la page en pouces de l'image de sortie.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/fr/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Le client peut contrôler le paramètre de page de l'imprimante lors de l'impression de chaque page à l'aide de cette fonction.|



###  Remarques



###  Voir également
* module [aspose.cells.rendering](..)
