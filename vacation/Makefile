VacationSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r16384 -t4096 >> VacationSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r16384 -t4096 >> VacationSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

VacationMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r1048576 -t4096 >> VacationMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r1048576 -t4096 >> VacationMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

VacationBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r1048576 -t4194304 >> VacationBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./vacation -n4 -q60 -u90 -r1048576 -t4194304 >> VacationBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu