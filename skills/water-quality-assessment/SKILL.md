---
name: water-quality-assessment
description: "Assess water quality data against the right standard and explain what it means. Use when given lab results or monitoring data for drinking water, river/surface water, groundwater, or mine/industrial effluent and asked whether it is safe, compliant, or trending worse. Produces a parameter-by-parameter comparison to a stated standard, an overall index, data-quality flags, likely causes, and next sampling steps. Flags that the applicable local regulation is the authority."
---

# Water-Quality Assessment

Turn a table of measurements into a defensible conclusion: compliant or not, against which standard, and what to do next.

## Required inputs (ask if missing)
- **Water type and use:** drinking, raw/surface water, groundwater, irrigation, mine effluent, or receiving water.
- **Applicable standard / jurisdiction.** Do not pick silently. If unstated, propose one and say so (e.g. WHO Guidelines for Drinking-water Quality for drinking water; for Indonesia, the national drinking-water regulation, the surface-water class system under PP 22/2021, and the sector effluent standard). Cite the instrument by name and tell the user to confirm the current version.
- **Data:** parameter, value, unit, sampling date/location, method or lab, detection limit.
- **Context:** upstream/downstream, rainfall, nearby activity (mining, agriculture, sewage).

## Method
1. **Check the data first.** Units consistent (mg/L vs µg/L), values below detection limit flagged (not treated as zero), total vs dissolved metals distinguished, holding times/preservation noted, field vs lab pH/DO/temperature. Report what is unreliable before judging.
2. **Compare each parameter to the standard.** Group: physical (pH, turbidity, TSS, conductivity/TDS, temperature), chemical (nitrate, ammonia, sulfate, chloride, hardness), metals (As, Pb, Cd, Hg, Fe, Mn, Cu, Zn, Cr), organic/oxygen (DO, BOD, COD), microbiological (E. coli / total coliform). State pass / exceed / below detection, and the margin.
3. **Separate health-based from aesthetic/operational limits.** Exceeding an aesthetic limit (e.g. taste, colour, iron) is not the same as a health hazard.
4. **Summarise with an index only if a method is specified** (e.g. NSF-WQI, or the Indonesian Pollution Index per KepmenLH 115/2003). Show the method and inputs; an index never replaces the per-parameter table.
5. **Interpret.** Link patterns to plausible causes (low pH + high sulfate + dissolved metals suggests acid mine drainage; high ammonia + coliform suggests sewage; high TSS after rain suggests erosion/runoff). Label these as hypotheses.
6. **Trend and spatial view** when multiple dates/sites exist: upstream vs downstream, seasonal change, direction of trend.
7. **Next steps:** resampling, additional parameters, confirmation lab, source investigation, treatment, or notification duty.

## Output format
**Scope & standard:** water type · standard used (confirm current version).
**Data quality flags:** list.
**Results table:** parameter | value | unit | limit | status.
**Overall conclusion:** compliant / exceedances / cannot conclude, in one sentence.
**Likely causes (hypotheses)** · **Recommended actions.**

> Local regulation and the accredited lab report are the authority. This is an interpretation aid, not a legal compliance determination. Do not declare water safe to drink from chemistry alone when microbiology is missing.

## Anti-patterns
- Comparing to a standard that does not fit the water's use.
- Treating non-detects as zero or ignoring detection limits above the standard.
- Declaring "safe" with missing parameters or unreliable data.
- Inventing limit values from memory; if unsure of a limit, say so and ask for the regulation text.
