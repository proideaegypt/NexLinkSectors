# Restore Instructions for v14

## Restoring the PDF index from GitHub chunks

1. Open the folder `versions/v14/chunks/`.
2. Concatenate all chunk files in lexical order.
3. Decode the resulting base64 text into a PDF file.

Example shell command:

```bash
cat ALL-SECTORS-PDF-INDEX-v14.pdf.base64.part* > ALL-SECTORS-PDF-INDEX-v14.pdf.base64
base64 -d ALL-SECTORS-PDF-INDEX-v14.pdf.base64 > ALL-SECTORS-PDF-INDEX-v14.pdf
```

## Artifact status

- PDF index: chunk-uploaded into the repo
- Main v14 zip: registered by manifest and checksum, not yet chunk-uploaded in this chat because of message-size limits
