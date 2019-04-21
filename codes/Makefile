all: raytrace cholesky fft lu-cb lu-nb ocean-cp ocean-np radix water-ns water-sp

raytrace:
	make -C ./apps/raytrace
cholesky:
	make -C ./kernels/cholesky
fft:
	make -C ./kernels/fft
lu-cb:
	make -C ./kernels/lu/contiguous_blocks
lu-nb:
	make -C ./kernels/lu/non_contiguous_blocks

# for ocean continguous
ocean-cp:
	make -C ./apps/ocean/contiguous_partitions
ocean-np:
	make -C ./apps/ocean/non_contiguous_partitions
radix:
	make -C ./kernels/radix
water-ns:
	make -C ./apps/water-nsquared
water-sp:
	make -C ./apps/water-spatial

clean:
	make -C ./apps/raytrace clean
	make -C ./kernels/cholesky clean
	make -C ./kernels/fft clean
	make -C ./kernels/lu/contiguous_blocks clean
	make -C ./kernels/lu/non_contiguous_blocks clean
	make -C ./apps/ocean/contiguous_partitions clean
	make -C ./apps/ocean/non_contiguous_partitions clean
	make -C ./kernels/radix clean
	make -C ./apps/water-nsquared clean
	make -C ./apps/water-spatial clean


