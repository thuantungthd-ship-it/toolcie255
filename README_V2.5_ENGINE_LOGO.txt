CIE V2.5 - LOGO EMBEDDED IN ENGINE
====================================

Two fixed logos are embedded directly in engine.py:
- DEFAULT_SIT_LOGO_B64
- DEFAULT_CIE_LOGO_B64

Helper:
    engine.get_logo_b64("SIT")
    engine.get_logo_b64("CIE")

No logo image file is required for these constants.

Streamlit main file:
    app.py

Note:
The current app.py remains backward-compatible with DEFAULT_LOGO_B64.
To make the UI selection actually switch the displayed/exported logo,
app.py must call engine.get_logo_b64(selected_logo) at the selection point.
