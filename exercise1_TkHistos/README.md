# POS2017 TRK-POS

## Exercise1 MultiTrackValidator and DQM

### SingleMuon phase1 vs phase0
1. bootstrap CMSSW_9_3_0
2. find workflows for SingleMu
3. run it for phas0 and phase1  (2000 events using 4 threads)
4. use MTV to produce comparison plots
5. load it to your web page and "analyze"

### TTbar tracking only reco+DQM
1. do a runTheMatrix dry-run (or -j0) for a phase1 (2017) wf TrackingOnly
2. copy step3 and step4 cfg 
3. identify a ttbar with pileup RAW file, use it as input for step3
4. harvest, mtv etc...

### tracking only reco+DQM on data
1. do a runTheMatrix dry-run (actually -j0) for a 2017 data wf
2. modify the reco+dqm step in "trackingOnly"
3. find a RAW data file fo 2017 (a recent run?)
4. run reco+dqm

### Bonus
1. create your own release area
2. download (git cms-addpkg) RecoTracker/IterativeTracking
3. mess-up with config
4. run reco+DQM+MTV and analyze the effect