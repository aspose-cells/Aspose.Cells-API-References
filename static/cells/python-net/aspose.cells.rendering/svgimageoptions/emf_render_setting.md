##emf_render_setting property
## emf_render_setting property
Setting for rendering Emf metafiles in source file.
### Remarks
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records.
Either type of record can be used to render the image, only EMF+ records, or only EMF records.
When [`EmfRenderSetting.EMF_PLUS_PREFER`](/cells/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed.
Default value is [`EmfRenderSetting.EMF_ONLY`](/cells/python-net/aspose.cells/emfrendersetting#EMF_ONLY).
For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
### Definition:
```python
@property
def emf_render_setting(self):
...
@emf_render_setting.setter
def emf_render_setting(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`EmfRenderSetting`](/cells/python-net/aspose.cells/emfrendersetting)
* class [`SvgImageOptions`](/cells/python-net/aspose.cells.rendering/svgimageoptions)
