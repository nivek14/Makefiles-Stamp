KmeansSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.05 -i random-n2048-d16-c16 -p $$t >> KmeansSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.05 -i random-n2048-d16-c16 -p $$t >> KmeansSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

KmeansMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.05 -i random-n16384-d24-c16 -p $$t >> KmeansMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.05 -i random-n16384-d24-c16 -p $$t >> KmeansMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

KmeansBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.00001 -i random-n65536-d32-c16 -p $$t >> KmeansBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./kmeans -m15 -n15 -t0.00001 -i random-n65536-d32-c16 -p $$t >> KmeansBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu