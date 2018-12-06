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
(base) C:\Windows\system32>conda create -n tenso
Solving environment: done


==> WARNING: A newer version of conda exists. <==
  current version: 4.4.10
  latest version: 4.5.11

Please update conda by running

    $ conda update -n base conda



## Package Plan ##

  environment location: C:\ProgramData\Anaconda3\envs\tenso


Proceed ([y]/n)? y

Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate tenso
#
# To deactivate an active environment, use
#
#     $ conda deactivate


(base) C:\Windows\system32>activate tenso

(tenso) C:\Windows\system32>pip install tensorflow-gpu==1.6.0
Collecting tensorflow-gpu==1.6.0
  Downloading https://files.pythonhosted.org/packages/89/65/73b33592e53ad205582cc800b72083012fb8335830bb3ac1533739db2983/tensorflow_gpu-1.6.0-cp36-cp36m-win_amd64.whl (85.9MB)
    100% |████████████████████████████████| 85.9MB 321kB/s
Collecting grpcio>=1.8.6 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/2f/bc/671ce1e13032cfaf6d4d8901019d376f8ce7f18ee046435bf18ee5782630/grpcio-1.17.0-cp36-cp36m-win_amd64.whl (1.5MB)
    100% |████████████████████████████████| 1.5MB 2.6MB/s
Requirement already satisfied: numpy>=1.13.3 in c:\programdata\anaconda3\lib\site-packages (from tensorflow-gpu==1.6.0)
Collecting protobuf>=3.4.0 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/e8/df/d606d07cff0fc8d22abcc54006c0247002d11a7f2d218eb008d48e76851d/protobuf-3.6.1-cp36-cp36m-win_amd64.whl (1.1MB)
    100% |████████████████████████████████| 1.1MB 2.4MB/s
Collecting termcolor>=1.1.0 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/8a/48/a76be51647d0eb9f10e2a4511bf3ffb8cc1e6b14e9e4fab46173aa79f981/termcolor-1.1.0.tar.gz
Collecting gast>=0.2.0 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/5c/78/ff794fcae2ce8aa6323e789d1f8b3b7765f601e7702726f430e814822b96/gast-0.2.0.tar.gz
Collecting astor>=0.6.0 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/35/6b/11530768cac581a12952a2aad00e1526b89d242d0b9f59534ef6e6a1752f/astor-0.7.1-py2.py3-none-any.whl
Collecting tensorboard<1.7.0,>=1.6.0 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/b0/67/a8c91665987d359211dcdca5c8b2a7c1e0876eb0702a4383c1e4ff76228d/tensorboard-1.6.0-py3-none-any.whl (3.0MB)
    100% |████████████████████████████████| 3.1MB 3.0MB/s
Collecting absl-py>=0.1.6 (from tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/0c/63/f505d2d4c21db849cf80bad517f0065a30be6b006b0a5637f1b95584a305/absl-py-0.6.1.tar.gz (94kB)
    100% |████████████████████████████████| 102kB 2.4MB/s
Requirement already satisfied: six>=1.10.0 in c:\programdata\anaconda3\lib\site-packages (from tensorflow-gpu==1.6.0)
Requirement already satisfied: wheel>=0.26 in c:\programdata\anaconda3\lib\site-packages (from tensorflow-gpu==1.6.0)
Requirement already satisfied: setuptools in c:\programdata\anaconda3\lib\site-packages (from protobuf>=3.4.0->tensorflow-gpu==1.6.0)
Collecting html5lib==0.9999999 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/ae/ae/bcb60402c60932b32dfaf19bb53870b29eda2cd17551ba5639219fb5ebf9/html5lib-0.9999999.tar.gz (889kB)
    100% |████████████████████████████████| 890kB 2.6MB/s
Collecting markdown>=2.6.8 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/7a/6b/5600647404ba15545ec37d2f7f58844d690baf2f81f3a60b862e48f29287/Markdown-3.0.1-py2.py3-none-any.whl (89kB)
    100% |████████████████████████████████| 92kB 2.5MB/s
Requirement already satisfied: werkzeug>=0.11.10 in c:\programdata\anaconda3\lib\site-packages (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu==1.6.0)
Collecting bleach==1.5.0 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu==1.6.0)
  Downloading https://files.pythonhosted.org/packages/33/70/86c5fec937ea4964184d4d6c4f0b9551564f821e1c3575907639036d9b90/bleach-1.5.0-py2.py3-none-any.whl
Building wheels for collected packages: termcolor, gast, absl-py, html5lib
  Running setup.py bdist_wheel for termcolor ... done
  Stored in directory: C:\Users\xbb123\AppData\Local\pip\Cache\wheels\7c\06\54\bc84598ba1daf8f970247f550b175aaaee85f68b4b0c5ab2c6
  Running setup.py bdist_wheel for gast ... done
  Stored in directory: C:\Users\xbb123\AppData\Local\pip\Cache\wheels\9a\1f\0e\3cde98113222b853e98fc0a8e9924480a3e25f1b4008cedb4f
  Running setup.py bdist_wheel for absl-py ... done
  Stored in directory: C:\Users\xbb123\AppData\Local\pip\Cache\wheels\18\ea\5e\e36e1b8739e78cd2eba0a08fdc602c2b16a4b263912af8cb64
  Running setup.py bdist_wheel for html5lib ... done
  Stored in directory: C:\Users\xbb123\AppData\Local\pip\Cache\wheels\50\ae\f9\d2b189788efcf61d1ee0e36045476735c838898eef1cad6e29
Successfully built termcolor gast absl-py html5lib
Installing collected packages: grpcio, protobuf, termcolor, gast, astor, html5lib, markdown, bleach, tensorboard, absl-py, tensorflow-gpu
  Found existing installation: html5lib 1.0.1
    Uninstalling html5lib-1.0.1:
      Successfully uninstalled html5lib-1.0.1
  Found existing installation: bleach 2.1.2
    Uninstalling bleach-2.1.2:
      Successfully uninstalled bleach-2.1.2
Successfully installed absl-py-0.6.1 astor-0.7.1 bleach-1.5.0 gast-0.2.0 grpcio-1.17.0 html5lib-0.9999999 markdown-3.0.1 protobuf-3.6.1 tensorboard-1.6.0 tensorflow-gpu-1.6.0 termcolor-1.1.0
You are using pip version 9.0.1, however version 18.1 is available.
You should consider upgrading via the 'python -m pip install --upgrade pip' command.

(tenso) C:\Windows\system32>
```


```
python
import tensorflow as tf
hello = tf.constant('Hello, Tensorflow!')
sess = tf.Session()
print(sess.run(hello))
```
