# gpower
import pandas as pd
import numpy as np
from statsmodels.stats.power import TTestIndPower
import matplotlib.pyplot as plt
pwr=0.8
d=0.75
alpha=0.05
power_analysis=TTestIndPower()
sample_size=power_analysis.solve_power(effect_size=d, power=pwr, alpha=alpha,nobs1 = None, alternative="two-sided")
print(sample_size)
