# Assemblers

1. MIRA
2. Velvet
3. ABYSS
4. SGA
5. SOAPdenovo
6. SPAdes
7. IDBA

# Assembly project

```yaml
basic_k: 23
joined_se_file: raw_reads.ok.keep.fast
```

# Single end data assembly

## Mira

## ABYSS

```bash
ABYSS -k23 -o ABYSS.k23.fa --coverage-hist=k23.coverage.txt -g k23.graph.dat -s k23.snp.dat -v  ../raw_reads.ok.fastq.fastq
```