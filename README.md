<p><pre align="center">
<strong>Variational Autoencoder: Alzheimer Detection Using Imbalanced MRI Images / <a href="https://www.youtube.com/channel/UCX7oe66V8zyFpAJyMfPL9VA">​Research Paper​</a></pre></p></strong>


### Abstract 

Alzheimer’s disease is an incurable, progressive neurologicaldisease  that  cause  the  brain  to  shrink  and  brain  cells  to  die.  Earlierdetection of Alzheimer’s disease can lead to proper treatment and pre-vent brain tissue damage. So accurate and fast detection of Alzheimer ismost important. There is many well established model which can predictAlzheimer’s disease but they struggle hard for imbalance datasets. Thiswork has foused on the early and fast detection of Alzheimer’s diseasefrom Imbalance Brain Magnetic resonance imaging(MRI) dataset usingproper Variational Autoencoder(VAE) model. Firstly, the whole datasethas been converted into a latent vector form then we used some popu-lar sampling methods to balance the dataset. Finally, we applied someclassification algorithm to classify the Brain MRI images into four dif-ferent classes‘Very Mild Demented’,‘Mild Demented’,‘Non Demented’and‘Moderate  Demented’.  In  order  to  maintain  the  stability  in  resultwe have applied 10-fold cross validation. In our experiment it indicatesimprovement in results to detect Alzheimer’s disease using VAE.

### Proposed Method

`Variational Autoencoder` <br>

In the case of Autoencoders the latent vector we get from the encoder part onlycontains  lattent  attributes  but  not  in  a  probabilistic  fashion.  That’s  why  we consider Variational Autoencoder(VAE)[10] for our experiment. VAE provide thelatent vector which contains lattent attributes as a probability distribution. Butin this consent a question may arise why not we are using Principal componentsanalysis(PCA) for the dimensionality reduction. The solution is, in the case ofdimensionality reduction PCA only perform linear dimensionality reduction butVAE  performs  large-scale  non-linear  dimensionalilty  reduction  also  VAE  canreduce the dimensionality fast and accurately without losing much information.The VAE model the input data as follows:
```
pθ(x|z) =f(x;z,θ)    p(z) =N(z|0,I)
```

<p align="center">
  <a href="https://www.youtube.com/channel/UCX7oe66V8zyFpAJyMfPL9VA">
    <img src="https://github.com/xiaowuc2/Variational-Autoencoder-Alzheimer-Detection/blob/main/Images/VAE.png" alt="Distribution">
</a>
  
<p align="center">Fig. 1 Variational Autoencoder is trained and Encoder is later used to obtainlatent vectors.</p>

`Latent Vector Resampling Techniques` <br>

Till  now  we  have  got  latent  vector  by  feeding  the  original  imbalance  data  toour  proposed  VAE.  Fig  2  depicts  how  our  proposed  VAE  is  generating  la-tent  vector  from  input  image  data.  In  this  section  we  are  mainly  focusing  onthe  trainning  biasing  problem  due  to  the  imbalance  in  the  dataset.  In  orderto  resolve  this  imbalance  problem  we  are  applying  some  popular  resamplingtechniques including, oversampling methods (Synthetic Minority OversamplingTechnique  (SMOTE)[6],  Adaptive  Synthetic  Sampling  (ADASYN)[9],  Borde-line  SMOTE[8](for  our  experiment  we  used  BorderlineSMOTE-1)  and  SVMSMOTE[13]) followed by some undersampling techniques (Cluster Centroid[20]. omek’s Links[16], Edited Nearest Neighbour(ENN)[18], Neighbourhood Clean-ing  Rule(NHC  Rule)[11]  and  All  KNN[15])  and  two  hybrid  sampling  methodviz., SMOTE ENN[2] and SMOTE Tomek[3]

<p align="center">
  <a href="https://www.youtube.com/channel/UCX7oe66V8zyFpAJyMfPL9VA">
    <img src="https://github.com/xiaowuc2/Variational-Autoencoder-Alzheimer-Detection/blob/main/Images/Enoder_VAE.png" alt="Distribution">
  </a>
  
<p align="center">Fig. 2 Proposed Encoder Architecture.</p>

### Citation

```

```
