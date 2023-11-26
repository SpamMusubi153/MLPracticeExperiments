# Fashion MNIST Architecture Tests

This notebook contains some of my deep learning experiments in the August of 2022 on the Fashion MNIST dataset. The dataset was loaded directly from Keras using their pre-defined training-validation split.

**My goal was to experiment broadly with model design and layer ordering**, rather than with fine-tuning hyperparameters and improving data for a specific model. Fashion MNIST seemed like a good next dataset to practice this on after I worked with MNIST through Jon Krohn's *Deep Learning Illustrated* book.

Each model experiment contains the code to build, compile, and train a model, followed by the verbose training output. Visualizations of each model are also included in the accompanying GitHub folder. 

My **highest validation accuracy of <ins>99.93%</ins>** was achieved in my **7th round of testing**.

Since I worked on these experiments, I've learned many new things about deep learning, model design, and using Jupyter notebooks that go quite a bit beyond the scope of these tests. I've decided, however, to publish a re-polished version of these tests **to show how far I've come since one of my first end-to-end deep learning projects** - that was not for a book or a class - as well as to **provide some reference code for others just getting started**.

**Good luck on your Deep ML Journey!**

Max Tran

---

**After I finished these tests, two things I wrote down that I had learned include:**

- Increasing kernel size (such as from 2x2 to 3x3 to 4x4, then 5x5) in a string of convolutional layers or blocks appears better than keeping the kernel size small and the same (such as by 2x2, 2x2, 2x2, 2x2).
- It seemed like convolutional and dense layers must be paired for maximum effectiveness. When I attempted to add a prediction step after the convolutional feature extractor, but before the dense classifier (in an attempt to provide information more directly to the convolutional layers) maximum validation accuracy seemed to decrease.