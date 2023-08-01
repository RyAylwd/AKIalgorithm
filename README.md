# AKIalgorithm
AKI detection based on KDIGO creatinine criteria
this algorithm assesses longitudinal creatinine results and stages each creatinine as 0, 1, 2 or 3.

Baseline creatinine:
Lookback:
median within 365 days
lowest within 7 days
lowest with 2 days (26.5 umol/L rule)

the index creatinine is compared to the lowest baseline value defined above
NB the baseline is fixed for the duration of the AKI episode to the baseline that triggered the AKI in the first place
the baseline assessment period resets after the end of the AKI episode, ie results from before and during the episode are removed and not considered in the detection of subsequent AKI
this is so that the creatinine results are not 'contaminated' with spuriously high results which will inflate the baseline and also recognises that the creatinine may not be the same compare to before the AKI

Start and end of the episode:
the AKi episode starts when a creatinine meets KDIGO criteria for the first time
the episode is automatically closed 7 days after the start of the AKI start, in keeping with the consensus that AKI lasts <= 7 days, after which acute kidney disease develops

Recovery assessment:
the most recent creatinine within the 7 day AKI episode is assessed for recovery.
status: complete, partial, nonrecovery, untested (see Simon Sawhney et al)
