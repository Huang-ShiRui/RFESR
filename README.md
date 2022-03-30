## RFESR


Code for our method Residual Feature Extraction Network for Ntire 2022 Efficient Super-Resolution Challenge

The model files are uploaded!  We use the [EDSR framework](https://github.com/sanghyun-son/EDSR-PyTorch) to train our RFESR and use the [IMDN test code](https://github.com/ofsoundof/IMDN) to reproduce results. To test our method,  you can run test_demo.py to get results in the challenge.

To avoid blocking effects appeared in the SR images, you have to modify the function tensor2int and int2tensor in the utils/utils_image.py to keep the range of the input images to [0, 255] instead of normalizing to [0, 1] as in the official test code.
