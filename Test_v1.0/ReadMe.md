### Event finder test v1.0

Performs:
- flatness test
- bump test
- pspl
- determination of microlensing candidate based off those tests

see [plots](https://KatieVandorou.github.io/Event_Finder/Test_v1.0/event_finder_2018DC.html) made from the 2018 Data Challenge. 

Metrics are reported in filename "2018DC_metric.md" or "2018DC_metric.tsv". The columns include:

- name of event
- "is_candidate": True/False
- "best_season": which Roman season (1-6) contains the candidate microlensing event
- "is_non_flat": for each season, is there a significant deviation from flatness (True/False)
- "bump_flag": for each season, for each window, does the lightcurve show statistically significant localised excess over that timescale. Window sizes: 2, 5, 10, 20, 50 days (True/False)
- "bump_snr": bump-feature signal-to-noise ratio.
- "best_window": which window size was best
- "chi2_red": reduced chi2 of the data against a constant flux model - for each season how inconsistent is the light curve with being flat overall.
- "t0_fit": time of peak magnification from PSPL (days)
- "u0_fit": source impact parameter from PSPL
- "tE_fit": Einstein ring radius (days)
- "chi2_red_pspl": reduced chi2 for pspl fit
