# [Python] Python Windows 개발 환경 구성 - anaconda python 설치

# 설치버젼
- `TENSORFLOW 1.6 설치 + PYTHON 3.6 설치 + CUDA 9.1 설치 + ANACONDA 5.1 설치 + CUDNN 7.1.1 설치 + JUPYTER NOTEBOOK으로 TENSORFLOW 이용` [참고 블로그](http://giyeon.blogspot.com/2018/03/tensorflow-16-python-36-cuda-91.html)

## 공식링크
- [python link](https://pypi.org/project/tensorflow-gpu/1.6.0/)

- [tensorflow](https://www.tensorflow.org/install/gpu)
- [nvidia](https://developer.nvidia.com/rdp/cudnn-archive)
- [python](https://pypi.org/project/tensorflow-gpu/1.6.0/)


## 참고사이트
- [cuda9.0](https://devyurim.github.io/python/tensorflow/2018/04/30/tensorflow-1.html)
- [Anaconda Tensorflow GPU 버전 설치 (2018.3)](https://junn.in/archives/2466)
- http://pubdata.tistory.com/94
- https://dwfox.tistory.com/67
- http://friday.fun25.co.kr/blog/?p=318
- http://giyeon.blogspot.com/2018/03/tensorflow-16-python-36-cuda-91.html
- http://eehoeskrap.tistory.com/225
- https://webnautes.tistory.com/1173





```
python
import tensorflow as tf
hello = tf.constant('Hello, Tensorflow!')
sess = tf.Session()
print(sess.run(hello))
```
