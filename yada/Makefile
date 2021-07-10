YadaSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./yada -a20 -i 633.2 -t $$t >> YadaSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./yada -a20 -i 633.2 -t $$t >> YadaSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

YadaMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./yada -a10 -i ttimeu10000.2 -t $$t >> YadaMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./yada -a10 -i ttimeu10000.2 -t $$t >> YadaMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

YadaBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./yada -a15 -i ttimeu1000000.2 -t $$t >> YadaBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./yada -a15 -i ttimeu1000000.2 -t $$t >> YadaBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu