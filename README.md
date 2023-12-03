# FINAL PROJECT TITLE HERE

## Project Description
Please describe your Startup Campus final project here. You may should your <b>model architecture</b> in JPEG or GIF.

## Contributor
| Full Name                | Affiliation                       | Email                          | LinkedIn                                       | Role          |
|--------------------------|-----------------------------------|--------------------------------|------------------------------------------------|---------------|
| M. Haswin Anugrah Pratama| Startup Campus, AI Track          | ---                            | [Haswin Pratama](https://www.linkedin.com/in/haswinpratama/)   | Supervisor |
| Aditia Taqi Pratama      | Universitas Negeri Jakarta         | aditaqipratama.0608@gmail.com | [Aditia Taqi](http://www.linkedin.com/in/aditaqip)             | Team Lead  |
| Ardis Hibatul Hakim      | Universitas Gunadarma              | ardishakim@gmail.com | [Ardis Hibatul Hakim](https://www.linkedin.com/in/ardis-hibatul-hakim/) | Team Member |
| Kinanthi Putri Siwilopo  | Universitas Amikom Purwokerto      | putkinanthi123@gmail.com | [Kinanthi Putri Siwilopo](https://www.linkedin.com/in/kinanthi-putri-siwilopo-b88b9b217/) | Team Member  |
| Maharani Ria Sina     | Universitas Sebelas Maret Surakarta| maharaniria281@gmail.com | [Maharani Ria Sina](https://www.linkedin.com/in/maharani-ria-sina-893620237/) | Team Member |
| Vindi Sovia Anggita      | Politeknik Negeri Malang        | vindisovia21@gmail.com | [Vindi Sovia Anggita](https://www.linkedin.com/in/vindi-sovia-anggita/) | Team Member |
| Ahmad Yudiman Fauzi      | Universitas Garut               | ozzifauzi9@gmail.com | [Ahmad Yudiman Fauzi](https://www.linkedin.com/in/ahmad-yudiman-fauzi-02665a22a/) | Team Member |

## Setup
### Prerequisite Packages (Dependencies)
- pandas==2.1.0
- openai==0.28.0
- google-cloud-aiplatform==1.34.0
- google-cloud-bigquery==3.12.0
- ...
- ...

### Environment
| | |
| --- | --- |
| CPU | Example: Apple M3 Pro 12-core CPU |
| GPU | Example: Nvidia A100 (x1) |
| ROM | Example: 1 TB SSD |
| RAM | Example: 36 GB |
| OS | Example: macOS Sonoma v14.1.1 |

## Dataset
Describe your dataset information here. Provide a screenshot for some of your dataset samples (for example, if you're using CIFAR10 dataset, then show an image for each class).
- Link: [https://...](https://app.roboflow.com/finalproject-uucte/keranjang-deteksi/16)

## Results
### Model Performance
Describe all results found in your final project experiments, including hyperparameters tuning and architecture modification performances. Put it into table format. Please show pictures (of model accuracy, loss, etc.) for more clarity.
![results](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/910b66f4-a0c9-4c5d-8369-9fbf70734bea)
![confusion_matrix](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/f7edb61e-f38a-43b7-aebe-18924fe34561)
![confusion_matrix_yolov5](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/71f8461e-8dd6-4163-a068-61d03b34a556)
![confusion_matrix_yolo7](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/fd183f3e-ee3b-4b6a-aadd-99de6ec59c22)
![PR_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/bb854481-ea16-42c7-9745-3a1018b52eb1)
![R_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/9c4653ce-7e6b-46c7-bccf-dfe155d11f3d)
![Precision_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/3d89251b-c2bf-4775-8194-d1895a76e652)


#### 1. Metrics
Inform your model validation performances, as follows:
- For classification tasks, use **Precision and Recall**.
- For object detection tasks, use **Precision and Recall**. Additionaly, you may also use **Intersection over Union (IoU)**.
- For image retrieval tasks, use **Precision and Recall**.
- For optical character recognition (OCR) tasks, use **Word Error Rate (WER) and Character Error Rate (CER)**.
- For adversarial-based generative tasks, use **Peak Signal-to-Noise Ratio (PNSR)**. Additionally, for specific GAN tasks,
  - For single-image super resolution (SISR) tasks, use **Structural Similarity Index Measure (SSIM)**.
  - For conditional image-to-image translation tasks (e.g., Pix2Pix), use **Inception Score**.

Feel free to adjust the columns in the table below.

| model | epoch | learning_rate | batch_size | optimizer | val_loss | val_precision | val_recall | ... |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| vit_b_16 | 1000 |  0.0001 | 32 | Adam | 0.093 | 88.34% | 84.15% | ... |
| vit_l_32 | 2500 | 0.00001 | 128 | SGD | 0.041 | 90.19% | 87.55% | ... |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | 

#### 2. Ablation Study
Any improvements or modifications of your base model, should be summarized in this table. Feel free to adjust the columns in the table below.

| model | layer_A | layer_B | layer_C | ... | top1_acc | top5_acc |
| --- | --- | --- | --- | --- | --- | --- |
| vit_b_16 | Conv(3x3, 64) x2 | Conv(3x3, 512) x3 | Conv(1x1, 2048) x3 | ... | 77.43% | 80.08% |
| vit_b_16 | Conv(3x3, 32) x3 | Conv(3x3, 128) x3 | Conv(1x1, 1028) x2 | ... | 72.11% | 76.84% |
| ... | ... | ... | ... | ... | ... | ... |

#### 3. Training/Validation Curve
Insert an image regarding your training and evaluation performances (especially their losses). The aim is to assess whether your model is fit, overfit, or underfit.
 
### Testing
Show some implementations (demos) of this model. Show **at least 10 images** of how your model performs on the testing data.

### Deployment (Optional)
Describe and show how you deploy this project (e.g., using Streamlit or Flask), if any.

## Supporting Documents
### Presentation Deck
- Link: [https://...](https://www.canva.com/design/DAF0gqaiBM4/wF7b4IWyKLsN5bwico1WuQ/edit)

### Business Model Canvas
Provide a screenshot of your Business Model Canvas (BMC). Give some explanations, if necessary.
![image](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/c9dc0e7b-6ece-4d2b-bca7-2d1c6223b221)
![image](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/f8946bab-d68b-43d7-9b09-c690854d8535)
![image](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/8f08e275-96a2-4275-a64e-0c0a6cb69ee4)
![image](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/5c7ef3a1-e1e8-4c55-a265-e5b2f50354ca)


### Short Video
Provide a link to your short video, that should includes the project background and how it works.
- Link: [https://...](https://drive.google.com/file/d/12eAYVySzJIBRrIhakdJoGINoz6rko_WW/view?usp=drivesdk)

## References
Provide all links that support this final project, i.e., papers, GitHub repositories, websites, etc.
- Link: [https://...](https://github.com/ultralytics/yolov5)
- Link: [https://...](https://www.businessinsider.com/how-british-startup-helped-uk-largest-retailers-luxury-improve-sales-2021-1)
- Link: [https://...](https://ieeexplore.ieee.org/Xplore/home.jsp)
- Link: [https://...](https://www.annualreports.com/HostedData/AnnualReportArchive/r/NYSE_RBS_2018.pdf)
- Link: [[https://...](https://www.statista.com/statistics/617136/digital-population-worldwide/#:~:text=Worldwide%20digital%20population%202023&text=As%20of%20October%202023%2C%20there,population%2C%20were%20social%20media%20users)

## Additional Comments
Provide your team's additional comments or final remarks for this project. For example,
1. ...
2. ...
3. ...

## How to Cite
If you find this project useful, we'd grateful if you cite this repository:
```
@article{
...
}
```

## License
For academic and non-commercial use only.

## Acknowledgement
This project entitled <b>"YOUR PROJECT TITLE HERE"</b> is supported and funded by Startup Campus Indonesia and Indonesian Ministry of Education and Culture through the "**Kampus Merdeka: Magang dan Studi Independen Bersertifikasi (MSIB)**" program.
