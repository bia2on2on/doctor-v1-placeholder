doctor-v1 — Release 1.0 origin
==============================

Source line
- Old repository: bia2on2on/doctor
- Base commit: c97714034e62b001a313ee6636b25d7bece9d374
- Base commit date: 2026-11-16T21:28:43Z
- The old repository is unchanged and remains the full-product line.

Release 1.0 scope (owner fixed, this independent line)
- Single-doctor clinic
- One doctor with several locations
- Building with independent clinics
- Patient panel
- SMS login and identity verification of patient
- Public booking
- Patient and medical-record management
- Scheduling and reception
- Visit recording
- Basic finance
- Security and RBAC
- Backup and restore

No code removed in this step.

Migration rule
- Migration numbers and text are decided in the old full line first.
- This line carries only migrations identical to the old line.
- Any new table/column needs explicit owner approval and a reserved identical
  migration in the old line.
- The only approved new table is cpms_patient_logins.

Security rule
- Every security fix must be applied to both lines by hand.
- Changes never flow automatically between lines.

Open owner items
- Replace example.local product URL (plugin header line 4) before release.
- Repository visibility: currently public; owner will make private later.
- Installer ZIP distribution.
- Which design documents to carry over (identity login, backup/restore).
- PR #357 test changes to carry over.
