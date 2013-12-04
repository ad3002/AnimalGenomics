# FastQC


# CEGMA

Cegma website: http://korflab.ucdavis.edu/datasets/cegma/

Alternatively you can use iplantcollaborative.org platform.

Installation instructions:

1. http://korflab.ucdavis.edu/datasets/cegma/ubuntu_instructions_1.txt
2. http://korflab.ucdavis.edu/datasets/cegma/ubuntu_instructions_2.txt

## CEGMA settings for other users:

To run CEGMA installation from other user you have to add following exports to your .profile file:

```bash
PATH=$PATH:/home/cegmauser/libs/geneid/bin/./
export CEGMA=/home/cegmauser/libs/cegma_v2.4.010312
export PERL5LIB="/usr/lib/perl/5.10:/home/cegmauser/libs/cegma_v2.4.010312/lib"
export WISECONFIGDIR=/home/cegmauser/libs/wise-2.4.1/wisecfg
export CEGMATMP="/home/youname/cegmatemp"
```

Then create directory with temporary files:

```bash
mkdir /home/youname/cegmatemp
```

Usage example for mammal genome:

```
cegma -g your_scaffolds.fa -p path_to/core.fa -o cegma.output_prefix -T 10 -v --ext --mam 
```

If you want to run several cegma processes than set unique temp directory for each of them.