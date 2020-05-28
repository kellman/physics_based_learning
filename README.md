# How to do Physics-based Learning

Computational imaging systems (_e.g._ tomographic systems, computational optics, magnetic resonance imaging) jointly design software and hardware to retrieve information which is not traditionally accessible. Generally, such systems are characterized by how the information is encoded (forward process) and decoded (inverse problem) from the measurements. Critical aspects of computational imaging systems, such as experimental design and image priors, can be optimized through deep networks formed by _unrolling_ the iterations of classical model-based reconstructions.

The goal of this open-source demonstration is provide a minimum working example for people new to physics-based learning to use it to design their own systems. With rapid prototyping in mind, we advocate exploiting the auto-differentiation functionalities in Pytorch twice, once to build ones physics-based network and again to perform physics-based learning. This will allow the user to only have to implement the forward model process for their system.

The IPython notebook contains a physics-based learning example that performs sparse recovery for an under-determined system, _i.e. compressed sensing_. We construct a physics-based network by unrolling the iterations of proximal gradient descent algorithm and perform physics-based learning to learn the system's measurement matrix, step size, and sparsity penalty.

For more details please refer to the document _How_to_do_Physics-based_Learning.pdf_.

If this is useful please [cite](https://arxiv.org/abs/2005.13531).