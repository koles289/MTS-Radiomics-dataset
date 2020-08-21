# MTS-Radiomics-dataset

Radiomics datasets created with python library Pyradiomics as part of the master thesis. The calculated features are from <b>BRATS challenge 2019</b>. <br>
It consist of over 300 samples, but the dataset is quite unbalanced as the number od scans of LGG tumours in dataset is around 70. <br>
The features are calculated using apriori provided mask of pathologic area in brain with selected different types of pathologic tissue. From this different parts of pathologic tissue are consequently created various  <b>Regions Of Interest (ROI)</b>. In the thesis, we used three ROI (ordered from smallest to largest area):
<ul>
  <li>1 - Non-enhancing tumopur witch necrotic area</li>
  <li>2 - hard core of tumour</li>
  <li>3 - Whole tumour with edem</li>
</ul>
The features comes from applying various filters to native images of brain - LoG filter, wavelet transform with various maternal waves and 3D LBP.</b>.
The various calculated fetures are in zip compressed files:
<ul>
  <li>Shape.zip - shape features calculated from native images and all three ROI</li>
  <li>bior15wave_log01108.zip - Features calculated using wavelet transform bior1.5 or LoG with alpha values of 0.11 or 0.8</li>
  <li>bior31wave_LBP.zip - Features calculated using wavelet transform bior3.1 or LBP</li>
  <li>coifwave_log0509.zip - Features calculated using wavelet transform coif wavelet or LoG with alpha values of 0.5 or 0.9</li>
</ul>


