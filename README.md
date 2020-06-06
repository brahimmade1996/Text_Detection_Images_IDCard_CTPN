# text-detection-ctpn

Scene text detection based on ctpn (connectionist text proposal network). It is implemented in tensorflow. The origin paper can be found [here](https://arxiv.org/abs/1609.03605). 

***
**NOTICE:I have to reonstruct this repo. The repo is written based on older dependencies**, such as 
- tensorflow-gpu==1.4.0 (to be upgraded to latest stable version - **tensorflow-gpu==1.12. 0** and **cuda==9.0** , the compatible **cuDNN version==7.1. 4**). 
- Model is saved in **hdf5** (not so optimized model servable / model serialization format). I'll re-factor the code with TF2.0, and save the model as **protobuff (.pb)** model serialization format.
- It's trained on **GTX1070 GPU**. I'm planning to retrain this on **TPU**.
- I'll reonstruct this repo with serving using **TF_Serving** for **Quantization and Pruning**.
***


# some results
`NOTICE:` all the photos used below are collected from the internet. If it affects you, please contact me to delete them.
<img src="/data/res/006.jpg" width=320 height=480 /><img src="/data/res/008.jpg" width=320 height=480 />
<img src="/data/res/009.jpg" width=320 height=480 /><img src="/data/res/010.png" width=320 height=320 />
***
## oriented text connector
- oriented text connector has been implemented, i's working, but still need futher improvement.
- left figure is the result for DETECT_MODE H, right figure for DETECT_MODE O
<img src="/data/res/007.jpg" width=320 height=240 /><img src="/data/res_oriented/007.jpg" width=320 height=240 />
<img src="/data/res/008.jpg" width=320 height=480 /><img src="/data/res_oriented/008.jpg" width=320 height=480 />
***
