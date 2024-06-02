# Eliptic-curve-with-multiprocessing
Am utilizat multiprocessing pentru operațiile realizate asupra unei curbe eliptice pentru a îmbunătății timpul necesar realizării acestor calcule.

Deoarece este necesarâ adunarea punctelor pe curba eliptică de multiple ori, ceea ce este o operațiune costisitoare computațional, se poate folosi un pool de procese pentru a aduna puncte în paralel utilizându-se nucleele sistemului pe care este rulat codul, reducând semnificativ timpul necesar pentru a obține rezultatul final.

Am utilizat o coadă pentru a gestiona comunicația între procese. Fiecare proces își depune rezultatul în coadă, iar după finalizarea tuturor proceselor, rezultatele sunt extrase și adunate. Acest mecanism de coadă asigură că procesele pot lucra în mod independent fără a interfera unele cu celălalt.
