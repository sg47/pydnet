# PyDnet
This repository contains the source code of pydnet, proposed in the paper "Towards real-time unsupervised monocular depth estimation on CPU", IROS 2018.
If you use this code in your projects, please cite our paper:

```
@inproceedings{pydnet18,
  title     = {Towards real-time unsupervised monocular depth estimation on CPU},
  author    = {Matteo Poggi and
               Filippo Aleotti and
               Fabio Tosi and
               Stefano Mattoccia},
  booktitle = {IEEE/JRS Conference on Intelligent Robots and Systems (IROS)},
  year = {2018}
}
```

For more details:
[arXiv](https://arxiv.org/abs/1806.11430)

Demo video:
[youtube](https://www.youtube.com/watch?v=Q6ao4Jrulns)

## Requirements

* `Tensorflow 1.8` (recomended) 
* `python packages` such as opencv, matplotlib

## Run pydnet on webcam stream

To run pydnet, just launch

```
python webcam.py --checkpoint_dir /checkpoint/IROS18/pydnet --resolution [1,2,3]
```

## Train pydnet from scratch

### Requirements

* `monodepth (https://github.com/mrharicot/monodepth)` framework by Clément Godard

After you have cloned the monodepth repository, add to it the scripts contained in `training_code` folder from this repository (you have to replace the original `monodepth_model.py` script).
Then you can train pydnet inside monodepth framework.
