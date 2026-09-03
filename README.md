# 3D Annotation Engine v0.1.0

Trimble Connect for Browser 3D Viewer extension.

## Install
1. Repository auf GitHub veröffentlichen.
2. GitHub Pages für den Root des Repositories aktivieren.
3. In `manifest.json` `YOUR-USERNAME` ersetzen.
4. In Trimble Connect: Project Settings → Apps & Capabilities → + Add Custom.
5. Als Capability Manifest URL die öffentliche `manifest.json` URL eintragen.

Manifest:
`https://YOUR-USERNAME.github.io/trimble-3d-annotation-engine/manifest.json`

Die Extension-URL im Manifest ist die URL der Web-App.

## v0.1
- TextMarkup
- Punkt-Picking über `viewer.onPicked`
- MeasurementMarkup
- 3D-Bemaßung aus LineMarkup + TextMarkup
- Auswahl und Objekt-Properties
- einfacher Stempel mit `{PropertyName}`-Platzhaltern
- Markups löschen

## Wichtige Einschränkung
Die öffentliche Workspace API ist nicht die SketchUp Ruby API. TextMarkup exponiert Text/Farbe/Picks, nicht Font, Texthöhe, Bold, Italic oder Extrusion. MeasurementMarkup exponiert Start/End und MainLineStart/MainLineEnd, aber kein dokumentiertes Text-Override-Feld.
