# TruthInsight harness session archive

A public, credential-redacted archive of the TruthInsightBench shared scientific-evidence harness experiments and their session records. The archive includes V1–V5 skill and prompt versions, five-task and Life_03 experiment artifacts, historical deliveries, scoring evidence, and a Chinese index.

The archive is split into two binary parts because GitHub imposes per-file limits. Git LFS is required to download the parts. After cloning with Git LFS, reconstruct the ZIP in the repository directory:

```sh
cat TruthInsight-public.zip.part-aa TruthInsight-public.zip.part-ab > TruthInsight-public.zip
shasum -a 256 -c SHA256SUMS
unzip TruthInsight-public.zip
```

The redacted archive retains the user's approved public content but replaces identified access tokens, passwords, and signing secrets, including occurrences in nested ZIPs. Some historical checksums no longer apply to files modified by redaction; use `SHA256SUMS.public` inside the reconstructed archive for this version. Automated pattern checks are not a guarantee that all possible sensitive content has been identified.
