BayesSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v32 -r1024 -n2 -p20 -i2 -e2 -t $$t >> BayesSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./bayes -v32 -r1024 -n2 -p20 -i2 -e2 -t $$t >> BayesSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

BayesMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v32 -r4096 -n2 -p20 -i2 -e2 -t $$t >> BayesMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./bayes -v32 -r4096 -n2 -p20 -i2 -e2 -t $$t >> BayesMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

BayesBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v32 -r4096 -n10 -p40 -i2 -e8 -s1 -t $$t >> BayesBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./bayes -v32 -r4096 -n10 -p40 -i2 -e8 -s1 -t $$t >> BayesBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu