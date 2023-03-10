---
title: SheetRender classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender classe
Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul à diverses images telles que (BMP, PNG, JPEG, TIFF..)
Le constructeur de cette classe , doit être utilisé après modification de pagesetup, style cellule.



Le type SheetRender expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | la construction de SheetRender, nécessite une feuille de calcul et ImageOrPrintOptions comme paramètres|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [page_count](/cells/fr/python-net/aspose.cells.rendering/sheetrender/page_count) | Obtient le nombre total de pages de la feuille de calcul actuelle.|
| [page_scale](/cells/fr/python-net/aspose.cells.rendering/sheetrender/page_scale) | Obtient l'échelle de page calculée de la feuille.<br/> Renvoie l'échelle définie si [PageSetup.zoom](/cells/fr/python-net/aspose.cells/pagesetup#zoom) est défini. Sinon, renvoie l'échelle calculée selon [PageSetup.fit_to_pages_wide](/cells/fr/python-net/aspose.cells/pagesetup#fit_to_pages_wide) et [PageSetup.fit_to_pages_tall](/cells/fr/python-net/aspose.cells/pagesetup#fit_to_pages_tall).|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [to_image(page_index, file_name)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Afficher certaines pages dans un fichier.|
| [to_image(page_index, stream)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Rendre certaines pages dans un flux.|
| [to_tiff(stream)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Rendre la feuille de calcul entière en tant qu'image Tiff à diffuser.|
| [to_tiff(filename)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Rendre la feuille de calcul entière en tant qu'image Tiff dans un fichier.|
| [to_printer(printer_name)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Rendre la feuille de calcul à l'imprimante|
| [to_printer(printer_name, job_name)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Rendre la feuille de calcul à l'imprimante|
| [to_printer(printer_settings)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Rendre la feuille de calcul à l'imprimante|
| [to_printer(printer_settings, job_name)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Rendre la feuille de calcul à l'imprimante|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Rendre la feuille de calcul à l'imprimante|
| [get_page_size_inch(page_index)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Obtenez la taille de la page en pouces de l'image de sortie.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/fr/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Le client peut contrôler le paramètre de page de l'imprimante lors de l'impression de chaque page à l'aide de cette fonction.|



###  Voir également
* module [aspose.cells.rendering](..)
