# Getting Started

1. Open an editor in your browser:
   - Value Streams: `editors/value-stream-editor-en-standalone.html`
   - Strategic Summary (Drivers/Goals/Objectives/Plans): `editors/strategic-summary-editor-en-standalone.html`
   - Business Processes (BPMN2): `editors/business-process-editor-en-standalone.html`
2. Fill in the data for the selected editor:
   - Value Streams: Summary and Canvas tabs
   - Strategic Summary: Drivers, Goals, Objectives (SMART), and Strategic Plans
3. Use **Import JSON** / **Export JSON** to iterate locally. Sample files are in `examples/`:
   - `examples/value-stream-template.json`
   - `examples/strategic-summary-template.json`
   - `examples/business-process-template.json`
4. Generate the **.dup** and import it into Essential (Open Source, Docker, or Cloud).

## Business Process Editor (BPMN2)

- Capture a hierarchical process list (ID, Name, Description) and attach a BPMN2 flow using the embedded modeler.
- Current limitation: the BPMN2 diagram is saved as a single `Diagram` instance; edits made directly to diagram elements after `.dup` import are not synchronized back to the underlying model.
- The Essential report has been adapted to show BPMN when opening “Business Process Flow”. To enable it, set the following in Protégé as shown in the provided screenshot:
  - Report XSL Filename
  - Context Page XSL Filename
- The customized XSL is available here: `assets/business-process-editor/report-xsl/core_bl_bus_process_model_bpmn.xsl`

Screenshots:

- Editor UI: `assets/business-process-editor/images/business-process-editor.png`
- Essential view: `assets/business-process-editor/images/essential-business-process-flow.png`
- Protégé configuration example: `assets/business-process-editor/images/protege-business-process-model.png`
