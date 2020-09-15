#### Ubuntu18.04 环境 编译tensorflow2.3

```shell
cd build_tensorflow/
docker build -t tf-arm -f Dockerfile .
docker run -it -v /tmp/tensorflow_pkg/:/tmp/tensorflow_pkg/ --env TF_PYTHON_VERSION=3.6 tf-arm ./build_tensorflow.sh configs/rk3399.conf 
```

