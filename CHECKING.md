# Checking in this contributor fork

Open **Actions → Contributor checks → Run workflow**. Leave the workflow branch
as `main`, set **check_ref** to a branch or immutable commit in this fork, and
choose a mode:

- `research-package`: runs one package's registered, bounded commands on Linux
  and Windows. Set **package** to its repository-relative directory and
  **check_ref** to the feature branch or commit. For the three-axis proof use
  `research/three-axis-sharp-cutoff` on `research-three-axis-kernel`. Only
  declared live inputs are materialized. Two commits of Git history cover this
  package's direct-main-parent pins; packages with older provenance may need
  more history and should fail rather than skip authentication.

- `sparse-tests`: runs the sparse-checkout regression tests on Linux and Windows,
  with ordinary and optimized Python 3.12. Start here for the setup repair on
  `fix-sparse-root-materialization`.
- `selected-metadata`: Linux source/hash and metadata check for the selected
  complete result. It downloads the declared input closure rather than every
  historical research package. A pass does not replay native operators or prove
  the multiplication theorem.

The workflow is manual, uses read-only repository permissions, and installs no
project dependencies beyond Python. The Actions logs record the checked commit.
Keep changes on topic branches and open PRs against `CrocSwap/integer-mult-bounds`.
The personal checking workflow is intentionally separate from those upstream PRs.

For mathematical work, first read `AGENTS.md`, `autoresearch.md` and the live
handoffs. `certificates/selected-result.json` identifies the reviewed complete
result and its full replay command. At setup, main commit
`32890bc5de034ab8fc93ac88ead7279a6a416d04` selects conditional
κ = `605457647/200000000000`. Pending component gains do not replace that record.

Full admission replay is separately budgeted: use the selected record's command
(currently `make frontier5413-verify`) in its supported environment. The manual
checks here deliberately do not trigger that large historical/physical replay.

For a local sparse checkout, use a current Git version. Windows may also require
repository-local `git config core.longpaths true`; its deeply nested research
capsules exceed normal path lengths. Never classify an actual deleted or changed
input as a harmless sparse omission. Run the emitted preflight command, then
the metadata baseline; the preflight itself authenticates no mathematical claim.

Prepared for Joseph Anglada with substantial OpenAI Codex assistance. Apache-2.0.
