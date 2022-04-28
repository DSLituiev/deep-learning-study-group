# deep-learning-study-group

## DALL-E2

### Technical References:
- CLIP ([Radford et al. (2021) Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020))
  - contrastive matching of text (BoW) and image embedding
  - task: find text-image pairs within a batch that match
 
- Contrastive Multiview Coding ([Tian, Krishnan, Isola, 2020](https://arxiv.org/abs/1906.05849))
  - task: find views of the same object within a batch
  - loss (exact): <img src="https://render.githubusercontent.com/render/math?math={\mathbb{E}{\log\frac{\rm{same\ pair}}{\rm{all\ pairs}}}}">
  - loss (approx v1): Noise-Contrastive Estimation
  - loss (approx v2): randomly sample *m* negatives and do a simple *(m+1)*-way softmax classification
- Diffusion CV models ([Ho, Jain, Abbeel, 2020](https://arxiv.org/abs/2006.11239), [Sohl-Dickstein, Weiss, Maheswaranathan, Ganguli, 2015](https://arxiv.org/abs/1503.03585))
