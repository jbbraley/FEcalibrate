## Calibration process

1. Create FE model
2. Gather test data
3. Choose responses to compare
4. Choose parameters that are uncertain and influential to responses
5. Run sensitivity studies to establish parameter value bounds
6. Setup calibration run
  1. Alter parameter values via FE API
  2. Run solver to produce results corresponding to test responses
  3. Pull FE solver responses
  4. Compare test responses to FE responses and condense to minimal metric
  5. Choose and employ optimization algorithm to find best parameter values to minimize comparison metric
7. Run calibration from different starting parameter values until certainty in the solution is established
8. Choose and save best calibration run


## Dependencies
[fileio](https://github.com/johndevitis/file)

[st7api](https://github.com/johndevitis/st7api)
