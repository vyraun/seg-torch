# Seg-Torch for Image Segmentation with Torch
This work is sparked as my personal research on simple segmentation methods
based on deep learning. It is the harvest of two great predecessors;

* https://github.com/e-lab/ENet-training
* https://github.com/fedor-chervinskii/segnet-torch
    * (real project page) http://mi.eng.cam.ac.uk/projects/segnet/

However this code includes radical differences (such as data loading, augmentation,
memory optimization) and it has more generic type of
implementation suitable to use for any custom project. You only need to modify
data-loader files ```data/custom-gen.lua``` and ```data/custom.lua.```

Be warned this is susseptcle to any bug. Any pull request is appriciated.

Check ```train_scripts/``` for example execution.

# Models
* <b>SegNet:</b> Very simple encoder-decoder network, segmenting end2end
* <b>EroNet:</b> Very similar but it chops Batch-Normalization and uses ELU
activation. It is below in accuracy but really-faster in training.

# Example Results
```exp_model/``` includes a proof of concept on CamVid dataset. If you compare
the results with the real-project this implementation has higher values
interestingly (at least for me) :) .

Model will be shared on Dropbox, as soon as I find some time to do so.
