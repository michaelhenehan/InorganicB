# InorganicB
Code from the Henehan et al. (2022, GCA) paper "No ion is an island: Multiple ions influence boron incorporation into CaCO3"
https://doi.org/10.1016/j.gca.2021.12.011
For those of you without priveleged access to the Elsevier Deathstar: http://www.michaelhenehan.science/HenehanGCA2021accepted.pdf

This code isn't the most polished, nor is it the most efficient! It relied on a lot of snippets of code shamelessly pinched (and corrupted?) from Oscar Branson, who I believe now has a much more efficient code for calling Pitzer in PHREEQC on his github. Beware that because of the way I've structured the code I think it calls and loads a separate PHREEQC instance for each Monte Carlo replicate, that ends up eating up RAM like DM vegan snackwursts. Hence my workaround (not having the time to dig in and write better code) was to export the first 1000 replicates to a csv file, then clearing the kernel and doing the next 1000, then loading both files and doing the plotting etc. It ain't pretty, but it got something done. 

Please feel free to contact me if you see any mistakes or have any constructive suggestions for making less crap code. 

Hope it's useful!
