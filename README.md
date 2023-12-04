# “Auto Total Card” Keranjang Penghitung Otomatis

## Project Description
“Auto Total Card” Keranjang Penghitung Otomatis is a system for efficiency and effectiveness in the retail business world, where this system can be implemented easily by every customer. Queues besides ruining the mood, queues also have quite a big financial impact on the retail world.
According to the results of several studies in Indonesia, as many as 26% of shop customers are reluctant to go to the shop again because the queues are quite long and not only that, the retail industry also loses several% of its customers, resulting in losses of 311 billion/year.
With these problems, we want to create an innovation that can help to solve the problem by creating an auto total card cart automatic counting project.
And the way this system works is that the customer goes to the mall/fruit shop then the customer chooses what fruit they want to consume and use, then the customer can directly scan the purchases that are already in their basket and input them into the system that we have created and the price will be returned. Each fruit can then scan the barcode to make payments using e-wallet

## Contributor
| Full Name                | Affiliation                       | Email                          | LinkedIn                                       | Role          |
|--------------------------|-----------------------------------|--------------------------------|------------------------------------------------|---------------|
| M. Haswin Anugrah Pratama| Startup Campus, AI Track          | ---                            | [Haswin Pratama](https://www.linkedin.com/in/haswinpratama/)   | Supervisor |
| Aditia Taqi Pratama      | Universitas Negeri Jakarta        | aditaqipratama.0608@gmail.com | [Aditia Taqi](http://www.linkedin.com/in/aditaqip)             | Team Lead  |
| Ardis Hibatul Hakim      | Universitas Gunadarma             | ardishakim@gmail.com | [Ardis Hibatul Hakim](https://www.linkedin.com/in/ardis-hibatul-hakim/) | Team Member |
| Kinanthi Putri Siwilopo  | Universitas Amikom Purwokerto | putkinanthi123@gmail.com | [Kinanthi Putri Siwilopo](https://www.linkedin.com/in/kinanthi-putri-siwilopo-b88b9b217/) | Team Member  |
| Maharani Ria Sina     | Universitas Sebelas Maret Surakarta| maharaniria281@gmail.com | [Maharani Ria Sina](https://www.linkedin.com/in/maharani-ria-sina-893620237/) | Team Member |
| Vindi Sovia Anggita      | Politeknik Negeri Malang        | vindisovia21@gmail.com | [Vindi Sovia Anggita](https://www.linkedin.com/in/vindi-sovia-anggita/) | Team Member |
| Ahmad Yudiman Fauzi      | Universitas Garut               | ozzifauzi9@gmail.com | [Ahmad Yudiman Fauzi](https://www.linkedin.com/in/ahmad-yudiman-fauzi-02665a22a/) | Team Member |

## Setup
### Prerequisite Packages (Dependencies)
# Base ----------------------------------------
- matplotlib>=3.2.2
- numpy>=1.18.5
- opencv-python
- Pillow>=7.1.2
- PyYAML>=5.3.1
- requests>=2.23.0
- scipy>=1.4.1  # Google Colab version
- torch>=1.7.0
- torchvision>=0.8.1
- tqdm>=4.41.0
- protobuf<4.21.5  # https://github.com/ultralytics/yolov5/issues/8012
- ultralytics
# Logging -------------------------------------
- tensorboard>=2.4.1
# Plotting ------------------------------------
- pandas>=1.1.4
- seaborn>=0.11.0
# Extras --------------------------------------
- ipython  # interactive notebook
- psutil  # system utilization
- thop  # FLOPs computation
- streamlit
- wget
- ffmpeg-python
- pyngrok
- streamlit_webrtc
- qrcode[pil]
- python-barcode

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
![confusion_matrix_yolov5](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/71f8461e-8dd6-4163-a068-61d03b34a556)
![confusion_matrix_yolo7](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/fd183f3e-ee3b-4b6a-aadd-99de6ec59c22)

#### 1. Metrics
Inform your model validation performances, as follows:
- For classification tasks, use **Precision and Recall**.
- For object detection tasks, use **Precision and Recall**. Additionaly, you may also use **Intersection over Union (IoU)**.
  ![PR_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/bb854481-ea16-42c7-9745-3a1018b52eb1)
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
![R_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/9c4653ce-7e6b-46c7-bccf-dfe155d11f3d)
![Precision_curve](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/3d89251b-c2bf-4775-8194-d1895a76e652)
![results](https://github.com/VindiSovia/AutoTotalCard/assets/105348760/910b66f4-a0c9-4c5d-8369-9fbf70734bea)

### Testing
Show some implementations (demos) of this model. Show **at least 10 images** of how your model performs on the testing data.
![data10](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/20a951ce-f5d7-49de-b506-e01f4bb40ed8)
![data9](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/ee22b9fc-2010-4da2-9b50-d33660c56330)
![data8](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/a60b84eb-9cbc-4bed-b554-d2d013af0029)
![data7](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/40601f54-4dfa-48db-b90e-835314fd55d1)
![data6](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/8771d155-fca0-4e6a-ab7a-11641b569031)
![data5](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/782afcf0-e43a-497e-8b07-b6564844b31e)
![data4](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/567143a6-1695-4758-baab-903aaabbd9f2)
![data3](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/b5a648c9-a4a3-4d2b-8113-5ae01a060c53)
![data2](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/d7635d0b-55b1-47c2-bdf1-74f071f36f86)
![WhatsApp Image 2023-12-04 at 14 01 41](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/6da8ccbf-c605-45be-8a09-0d67986be2de)

### Deployment (Optional)
We make an application using the help of Streamlit. An example image will appear below
![gambar 1](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/0b38efea-e938-4ac5-94af-e8873337045a)
![gambar 2](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/be50a173-d40f-4f3c-9305-92a898130e6c)
![gambar 3](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/5dfcca2c-300e-4615-9db2-3a0ef421b9cf)
![gambar 4](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/e0990c6b-cff0-4279-82a7-fbc1697234d1)
![gambar 5](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/652b7be8-b0b5-4421-9517-dc8bb68a42b1)
![gambar 6](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/deccefb4-0d5e-4613-bb49-98a744a6768f)
![gambar 7](https://github.com/VindiSovia/AutoTotalCard/assets/75414611/8eedf654-b692-47d2-8cc2-aa578f12d222)
You can find the code in the folder or click the link below
Link: [https://...](https://colab.research.google.com/drive/1tTNMWKBhLJgvIThMfJNbDYhR1HVYoVLv?usp=sharing)

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
- Link: [[https://...](https://github.com/thepbordin/YOLOv5-Streamlit-Deployment)

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
This project entitled <b>"“Auto Total Card” Keranjang Penghitung Otomatis"</b> is supported and funded by Startup Campus Indonesia and Indonesian Ministry of Education and Culture through the "**Kampus Merdeka: Magang dan Studi Independen Bersertifikasi (MSIB)**" program.
