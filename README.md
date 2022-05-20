# LIMSimulator

## Purpose

To simulate systematics and data analysis pipelines for line intensity mapping experiments.

## Initial goals

Design goals was put together at HIIM workshop in Trieste 2022.
Goals:
 - Interface for reading in meta data (pointing/flags/etc...) from real experiments
   - Experiments of interest: MeerKLASS, COMAP, ...??
 - Implementation of a sky model:
   - Large-scales can you use PySM (>1 degree)
   - Small-scales assume gaussianity? All-sky maps interferometric surveys? (<1 degree)
 - Systematics to simulate:
   - Noise:
    - White noise
    - Correlated 1/f noise (atmospheric, receiver, frequency correlations)
    - Standing waves (possibly manifest as frequency correlated noise)
  - Instrument specific:
    - Polarisation leakage/faraday rotation
    - Ground pick-up
    - Standing waves (signal dependent?)
 - Pipeline simulations:
  - Basic implementations of data analysis pipelines, i.e.:
    - Filters
    - Calibration
    - Map-making
    - ??? 
