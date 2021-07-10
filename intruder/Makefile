IntruderSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./intruder -a10 -l4 -n2048 -s1 -t $$t >> IntruderSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./intruder -a10 -l4 -n2048 -s1 -t $$t >> IntruderSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

IntruderMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./intruder -a10 -l16 -n4096 -s1 -t $$t >> IntruderMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./intruder -a10 -l16 -n4096 -s1 -t $$t >> IntruderMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

IntruderBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./intruder -a10 -l128 -n262144 -s1 -t $$t >> IntruderBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./intruder -a10 -l128 -n262144 -s1 -t $$t >> IntruderBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu