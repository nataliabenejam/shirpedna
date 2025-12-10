REVAMP pipeline code

# FORCE X86_64

arch -x86_64 zsh

# RUN EXPORT PATH WITH LOWERCASE S FOR REVAMP.SH TO WORK

export PATH=~/software/REVAMP:$PATH
which revamp.sh

# RUN EXPORT PATH FOR BLASTN TO WORK

export PATH=~/software/blast-2.13/bin:$PATH
which blastn

# TAXONKIT PATH

export TAXONKIT_DB=~/.taxonkit

# KRONA PATH

export PATH=$HOME/software/KronaTools-2.7.1/bin:$PATH
which ktImportKrona

export PATH=~/software/KronaTools-2.7.1/scripts:$PATH
which ImportText.pl

# CD INTO SHIRPEDNA

cd /Volumes/NB/shirpeDNA 

# THEN RUN THIS TO BEGIN REVAMP

revamp.sh -p 01_config_file_MiFish_2025a.txt -f 02_figure_config_file_MiFish_2025a.txt -s 03_sample_metadata_MiFish_2025a.txt -r 2025_mifish_raw/2025fastqa -o results_revamp_MiFish_2025a -t 1

revamp.sh -p 01_config_file_MiFish_2025b.txt -f 02_figure_config_file_MiFish_2025b.txt -s 03_sample_metadata_MiFish_2025b.txt -r 2025_mifish_raw/2025fastqb -o results_revamp_MiFish_2025b -t 1

revamp.sh -p 01_config_file_MiFish_2025c.txt -f 02_figure_config_file_MiFish_2025c.txt -s 03_sample_metadata_MiFish_2025c.txt -r 2025_mifish_raw/2025fastqc -o results_revamp_MiFish_2025c -t 1

revamp.sh -p 01_config_file_Elas02_2025a.txt -f 02_figure_config_file_Elas02_2025a.txt -s 03_sample_metadata_Elas02_2025a.txt -r 2025_elas02_raw/2025fastqa -o results_revamp_Elas02_2025a -t 1

revamp.sh -p 01_config_file_Elas02_2025b.txt -f 02_figure_config_file_Elas02_2025b.txt -s 03_sample_metadata_Elas02_2025b.txt -r 2025_elas02_raw/2025fastqb -o results_revamp_Elas02_2025b -t 1
