Supplementary data for Ritchie AM, Hua X, Bromham L (2021) Investigating the reliability of molecular estimates of evolutionary time when substitution rates and speciation rates vary

This data set includes:

simulated_trees: Files containing simulated data sets of 50 phylogenetic trees in Newick format. Trees were simulated under three simulation models:
			Unlinked - speciation and substitution rates vary independently and are autocorrelated along lineages 
			Continuous - speciation and substitution rates vary continuously as a multivariate Brownian motion with nonzero covariance
			Punctuated - speciation and substitution rates vary independently. Bursts of substitutions occur after each speciation event. 

simulated_alignments: FASTA files containing nucleotide alignments simulated along the correspondingly numbered trees under an HKY model with parameters derived from 
			Barker et al. (2012) Plos One 7(10):e46403.

beast_reconstructed_trees: Trees reconstructed from simulated alignments under the Uncorrelated Lognormal Relaxed Clock (UCLN) in BEAST 2. 
	
	beast_xmls: XML control files for all analyses in BEAST 2, including calibrations and prior distributions.
				

paml_reconstructed_trees: Trees reconstructed from simulated trees and aligments under the Autocorrelated Lognormal Relaxed Clock (ACLN) in mcmctree, part of the PAML 4 suite.

	Code_control_files: 	R functions for simulating sampled trees with covarying speciation and substitution rates (bdforward.R)
				Example control files for PAML (Unlinked_1.ctl,Unlinked_1_run2.ctl)
				paml_trees: Calibrated tree topologies without branch lengths for PAML node time reconstruction
				