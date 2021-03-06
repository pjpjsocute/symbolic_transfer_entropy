# Symbolic Transfer Entropy

My implementation of Symbolic Transfer Entropy -- a method of estimating transfer entropy which was proposed in

[Symbolic Transfer Entropy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.100.158101)

Matthaus Staniek and Klaus Lehnertz 2008

## Files 

In the order of which they were used:

1. coupled_lorenz.m 
    + integrates coupled lorenz systems and stores time series data in lorenz_data/ (too big; not included in repository)
    + each saved file corresponds to one simulation (i.e. one initial condition)
        - each pair of columns corresponds to one coupling parameter
        - odd columns correspond to driver (x), even columns correspond to response (y)
2. coupled_rossler.m
    + same as coupled_lorenz.m but with rossler systems
3. symbolic_TE.py
    + my implementation of Symbolic Transfer Entropy (STE)
4. TE_test.py 
    + computes STE for lorenz system and rossler system
    + stores entropies in lorenz_entropies.csv and rossler_entropies.csv  
5. TE_plot.py
    + recreates figures from paper
    + resulting figures are saved in figs/
