# btMSI-CAST

b/tMSI-CAST (blood/tissue MSI Caller Adjusted with Sequence duplicaTes), an NGS-based composite MSI detection method that has a two-mode caller compatible with both tissue and plasma samples and does not require matched normal samples.


# Usage
Version 0.10
Usage:  msicast <mode> [options]

## modes
dedup_only   <string>    perform duplication removal only.
deletion-ratio   <string>    MSI calling under the deletion-ratio mode.
kld   <string>    MSI calling under the kld mode.

## options
-- inbam (-i)   <string>    input BAM file
-- outprefix (-o)   <string>    prefix for a series of output files
    
-c   <int>      coverage threshold for msi analysis, default=20
-b   <int>      threads number for parallel computing, default=1
-y   <int>      output microsatellite only, 0: no; 1: yes, default=0

# Example

take pre-deduplication BAMs as input and perform duplication removal by a proprietary majority-voting strategy.



# Contact
If you have any questions, please contact one or more of the following folks: Beifang Niu bniu@sccas.cn Xinyin Han hanxinyin@cnic.cn
