# running cifar10 example
1. in caffe-error-injection-knl dir
2. cp -r cifar10/*lmdb /dev/shm/
3. cp cifar10/mean.binaryproto /dev/shm/
4. build/tools/caffe.bin train -engine "MKL2017" --solver=model/cifar10/cifar10_full_solver.prototxt

