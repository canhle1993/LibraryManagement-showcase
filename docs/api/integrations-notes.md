# External Integrations Notes

This project is a **desktop application**, so the "API" aspect is mainly about external libraries and service integrations rather than public REST endpoints.

## Vbee Text-To-Speech

The project includes a feature where users can open a book description and click the speaker icon to hear an audio narration.

- Input: book description text
- Service: Vbee text-to-speech API
- Output: generated audio file stored locally before playback
- User value: improves accessibility and creates a richer book-detail experience

## QR Code / Barcode Workflow

The warehouse and inventory workflow supports QR-based scanning.

- QR decoding library: ZXing
- Camera support: phone camera via DroidCam
- Media handling: OpenCV / JavaCV / FFmpeg
- Result: scanned book codes can be matched with inventory records and used in warehouse verification workflows

## Reporting

The project also uses reporting-oriented libraries:

- JasperReports for exporting or generating structured report output
- Apache POI for spreadsheet-related workflows

## Notes For Reviewers

- This repository does not expose private service credentials or implementation code
- The purpose here is to explain the integration surface and the role each external tool plays in the product
