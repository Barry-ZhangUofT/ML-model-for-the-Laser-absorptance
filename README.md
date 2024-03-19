Paper-Laser absorptance prediction

Laser absorptance prediction models for the paper Accurate predictions of keyhole depths using machine learning-aided simulations" by Jiahui Zhang, Runbo Jiang, Kangming Li, Pengyu Chen, Xiao Shang, Zhiying Liu, Jason Hattrick-Simpers, Brian J. Simonds, Qianglong Wei, Hongze Wang, Tao Sun, Anthony D. Rollett, Yu Zou. The abstract of the paper is as follows:

"The keyhole phenomenon is widely observed in laser materials processing, including laser welding, remelting, cladding, drilling, and additive manufacturing. Keyhole-induced defects, primarily pores, dramatically affect the performance of final products, impeding the broad use of these laser-based technologies. The formation of these pores is typically associated with the dynamic behavior of the keyhole. So far, the accurate characterization and prediction of keyhole features, particularly keyhole depth, as a function of time has been a challenging task. In situ characterization of keyhole dynamic behavior using a synchrotron X-ray is complicated and expensive. Current simulations are hindered by their poor accuracies in predicting keyhole depths due to the lack of real-time laser absorptance data. Here, we develop a machine learning-aided simulation method that attains unprecedented accuracy for predicting keyhole depth over a wide range of processing parameters. Based on titanium and aluminum alloys, two commonly used engineering materials as examples, we achieve an accuracy with an error margin of 10 %, surpassing those simulated using other existing models (with an error margin in a range of 50-200 %). This exceptional fidelity empowers our model to serve as a cost-effective alternative to synchrotron experiments. Our machine learning-aided simulation method is affordable and readily deployable for a large variety of materials, opening new doors to eliminate or reduce defects for a wide range of laser materials processing techniques."

Data:
The derived laser absorptance data has already been submitted as supplementary Data to the journal. The experimental absorption datasets can be made available upon reasonable request to B.J.S. The X-ray dataset can be made available upon reasonable request to A.D.R. The dataset of segmented keyhole images can be made available upon reasonable request to Y.Z. 

Description:
These two Gaussian process regression models are established to predict laser absorptance based on processing parameters (P(W); v(mm/s); ro(μm)) for Ti-6Al-4V and Al6061. Models are trained based on the regression learner via MATLAB 2022.

Demo:
Take an example: predict the laser absorptance value for Ti64 under 500W power; 600mm/s scan speed; 50micron laser spot radius. Download the GPRTi.mat file and import into MATLAB 2022.

"X=[540,600,50];
YPredict=TiGPR.predictFcn(X);"
