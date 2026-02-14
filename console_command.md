
#### ProteoWizard
<pre><code>cd /d C:\Users\type\Desktop\MS\raw && for %f in (*.raw) do "C:\Program Files\ProteoWizard\ProteoWizard 3.0.26045.5b88a22\msconvert.exe" "%f" --mzML --filter "peakPicking true 1-" --zlib -o "."</code></pre>

#### Minimap

<pre><code>minimap2 -t 32 -ax map-ont /Bmo/jyakovleva/Panshin/out_nano/assembly.fasta \ 
/Bmo/jyakovleva/Panshin/oper/len1000_filtered.fastq > /Bmo/jyakovleva/Panshin/oper/aln1.sam</code></pre>

#### Quast

<pre><code>quast.py -o /Bmo/jyakovleva/Panshin/oper/quast_output -r /Bmo/jyakovleva/Panshin/oper/len1000_filtered.fastq \
-g /Bmo/jyakovleva/Panshin/oper/first_cycle/medaka_1/consensus.fasta /Bmo/jyakovleva/Panshin/oper/second_circle/medaka_11/consensus.fasta \ 
/Bmo/jyakovleva/Panshin/oper/third_cycle/medaka_3/consensus.fasta</code></pre>

#### Proteinortho

<pre><code>proteinortho -cpus=16 -ram=25 -project=preeria *.faa 40-19</code></pre>
