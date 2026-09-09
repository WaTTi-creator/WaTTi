# Lovable Import Branch

This branch is reserved for the first complete synchronization of the existing Lovable application.

Source checkpoint: `87cba50f0a0af8d697e38e54c3f4b687f086d5a4`

Rules:
- Import the real Lovable source; do not reconstruct it.
- Keep `main` untouched during import.
- Verify the complete source tree, including binary assets, before merging.
- Run dependency installation, typecheck, lint, and production build after the complete tree is present.
- Merge only after verification.
