LabyrinthSmall:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./labyrinth -i random-x32-y32-z3-n96 -t $$t >> LabyrinthSmallOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./labyrinth -i random-x32-y32-z3-n96 -t $$t >> LabyrinthSmallOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

LabyrinthMedium:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./labyrinth -i random-x48-y48-z3-n64 -t $$t >> LabyrinthMediumOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./labyrinth -i random-x48-y48-z3-n64 -t $$t >> LabyrinthMediumOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

LabyrinthBig:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./labyrinth -i random-x512-y512-z7-n512 -t $$t >> LabyrinthBigOutTiny$$t.txt ; \
			#OMP_NUM_THREADS=$$t ./labyrinth -i random-x512-y512-z7-n512 -t $$t >> LabyrinthBigOutSwiss$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu