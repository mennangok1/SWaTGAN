# SWaTGAN
Term Project for CS485 Deep Generative Networks Course

IN this project, we propose the novel architecture Sliding Window Attention-GAN (SWaTGAN), which utilizes sliding window attention (SWA) layers, from [2]. Initially proposed for natural language processing tasks, SWA limits the receptive field of each token to a predetermined window size. In this way, in the early layers of transformer blocks, the similarity score is calculated between the nearby tokens. The receptive field of each token increases towards the latter transformer layers, enabling the model to capture long-range dependencies despite starting with a narrow receptive field. Using SWA enables SWaTGAN to achieve a competitive performance in unconditional image generation tasks in a more efficient way than vanilla transformer based architectures. We trained SWaTGAN model with CelebA dataset, taken from Kaggle [7], which contains celebrity face images. We also trained TransGAN [4], and DCGAN [3] models with the same dataset in order to compare the results, and the training times of these models.



## References
[1] Goodfellow, I., Pouget-Abadie, J., Mirza, M., Xu, B., Warde-Farley, D., Ozair, S., Courville, A., & Bengio, Y. (2014). Generative adversarial nets. In Advances in neural information processing systems (pp. 2672-2680).

[2] Beltagy, I., Peters, M. E., & Cohan, A. (2020). Longformer: The Long- Document Transformer. arXiv preprint arXiv:2004.05150.

[3] Radford, A., Metz, L., & Chintala, S. (2015). Unsupervised Representa- tion Learning with Deep Convolutional Generative Adversarial Networks. arXiv preprint arXiv:1511.06434.

[4] Jiang, Y., Chang, S., & Wang, Z. (2021) TransGAN: Two Pure Transformers Can Make One Strong GAN, and That Can Scale Up. [Online]. Available: arXiv:2102.07074v1

[5] Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., Kaiser, Ł., & Polosukhin, I. (2017). Attention Is All You Need. arXiv preprint arXiv:1706.03762.

[6] Dosovitskiy, A., Beyer, L., Kolesnikov, A., Weissenborn, D., Zhai, X., Unterthiner, T., Dehghani, M., Minderer, M., Heigold, G., Gelly, S., Uszkoreit, J., & Houlsby, N. (2020). An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale. arXiv preprint arXiv:2010.11929.

[7] https://www.kaggle.com/datasets/jessicali9530/celeba-dataset/

[8] Karras, T., Aila, T., Laine, S., Lehtinen, J. (2018). Progressive Growing of GANs for Improved Quality, Stability, and Variation. arXiv preprint
arXiv:1710.10196.
