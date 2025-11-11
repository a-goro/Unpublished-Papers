# Unpublished-Papers

## Proof of Ownership Disclaimer

The files in this repository serve as a **cryptographic proof of ownership** for the PDF file `signed_paper.pdf`.  
**Important:** The PDF itself is **not included** and remains private. These files only prove that the PDF existed in its current form at the time the proof was created.

- `document-proof.txt` — Ownership statement + SHA-512 hash + timestamp  
- `document-proof.txt.asc` — Detached PGP signature of the proof text  
- `asel_goro_public.asc` — Public key for signature verification  

Anyone can use these files to **verify that the PDF exists and is authored by Asel Goro** without revealing its contents.

---

## How to Verify the Proof

### Import the public key

gpg --import asel_goro_public.asc
gpg --verify document-proof.txt.asc document-proof.txt

the paper would then be verified using : sha512sum signed_paper.pdf
