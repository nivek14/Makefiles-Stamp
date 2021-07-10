Ssca2Small:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./ssca2 -s13 -i1.0 -u1.0 -l3 -p3 -t $$t >> SSCA2SmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./ssca2 -s13 -i1.0 -u1.0 -l3 -p3 -t $$t >> SSCA2SmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

Ssca2Medium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./ssca2 -s14 -i1.0 -u1.0 -l9 -p9 -t $$t >> SSCA2MediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./ssca2 -s14 -i1.0 -u1.0 -l9 -p9 -t $$t >> SSCA2MediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

Ssca2Big:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./ssca2 -s20 -i1.0 -u1.0 -l3 -p3 -t $$t >> SSCA2BigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./ssca2 -s20 -i1.0 -u1.0 -l3 -p3 -t $$t >> SSCA2BigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu