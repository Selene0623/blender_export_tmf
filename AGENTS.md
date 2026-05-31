# blender_export_tmf - AGENTS.md

## Development & Testing

**Install in Blender:**
1. Open Blender
2. Edit → Preferences → Add-ons → Install
3. Select `3ds_export_tmf.py`
4. Enable the add-on

**Export workflow:**
- File → Export → 3DS for TMF (.3ds)
- Use "Selection Only" to export selected objects
- Outputs .3ds file compatible with TrackMania Forever

**Testing tips:**
- Test with simple meshes first (cube, UV sphere)
- Verify UV textures export correctly
- Check object hierarchy/transforms are preserved
- Validate output in TMF or 3DS viewer

**Important notes:**
- Single-file add-on - all logic in `3ds_export_tmf.py`
- No build/test/CI setup required
- Currently updated to Blender 5.1.2 API (see bl_info in 3ds_export_tmf.py)
- May require additional API adjustments for full compatibility
- GPL licensed