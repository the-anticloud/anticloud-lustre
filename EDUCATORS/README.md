# Educators — LUSTRE

**Project:** LUSTRE  
**Category:** SUPERCOMPUTER  
**Upstream:** see BENCH.json  
**Pinned commit:** `f5ac432bb2d625951be4f8731fe446aa03320061`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5eb8ba834ed37a162663af2fc8c51313ba2306e9d1398833359d0f43c2a6e4d2`  
**Date:** October 2026

## Teaching with LUSTRE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `5eb8ba834ed37a162663af2fc8c51313ba2306e9d1398833359d0f43c2a6e4d2` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
