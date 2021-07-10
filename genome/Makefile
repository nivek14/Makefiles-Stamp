GenomeSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./genome -g256 -s16 -n16384 -t $$t >> GenomeSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./genome -g256 -s16 -n16384 -t $$t >> GenomeSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

GenomeMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./genome -g512 -s32 -n32768 -t $$t >> GenomeMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./genome -g512 -s32 -n32768 -t $$t >> GenomeMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

GenomeBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./genome -g16384 -s64 -n16777216 -t $$t >> GenomeBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./genome -g16384 -s64 -n16777216 -t $$t >> GenomeBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu