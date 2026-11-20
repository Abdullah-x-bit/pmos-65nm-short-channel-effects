# Known issues and open items

Found while assembling the repository. None change the qualitative conclusions, but they should be fixed or documented.

1. **Qss mismatch.** The report's scaling table lists Qss = 1×10¹⁰ cm⁻²; the deck sets `Qss = 5e10`.
2. **Temperature shift.** The extracted Vth table (−0.23174 V at 300 K, −0.12652 V at 550 K) is a shift of about 105 mV; the report text says "approximately 89 mV".
3. **Optimized design not in the deck.** The deck holds the baseline 65 nm parameters (xj = 60k nm, NSD = 1e19/k², Nsub = 1e18/k²). The values behind Ion = 329.9 µA / Ioff = 0.69 nA (xj = 240k nm, NSD = 10²¹ cm⁻³, ND = 1.2×10¹⁸/k² cm⁻³) are not reproducible from this file. 240k nm ≈ 173 nm also exceeds the deck's 144 nm substrate depth.
4. **Commented-out analyses.** The S/D junction-depth sweep (20/40/60/90 nm), μeff extraction, the DIBL Vt extraction (`VTP1`, `VTP2`, `DIBL`) and the second-VD C-V block are disabled. The Vt-vs-L, gm, gd and ro results have no deck section, so they were presumably post-processed or run from other decks.
5. **Broken extraction.** The `VDep_AT_TEMP_*` lines evaluate `probe."Electron Concentration" - probe."Electron Concentration"`, which is always zero.
6. **Leftovers.** The duplicated commented-out block uses NMOS-era `VTN*` names and a stale `DIBL` formula; electrode comments say "Polysilicon" where the material is `Alum`.
