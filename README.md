# SKKU Collaborative Project
2022학년도 성균관대학교 산학협력프로젝트

</br>

## Project
### Task
딥러닝 기반의 텍스트 마이닝 기술 개발 및 Django 기반 학습 구축 도구 개발
### Duration
2022.04 ~ 2022.12
### Members
|최진우|권동욱|류도현|김도현|허지원|
|:---:|:---:|:---:|:---:|:---:|
|성균관대학교 소프트웨어학과 3학년|성균관대학교 소프트웨어학과 3학년|성균관대학교 소프트웨어학과 3학년|성균관대학교 소프트웨어학과 2학년|성균관대학교 소프트웨어학과 2학년|

### About
자연어처리(감성분석, 개체명인식) 모델의 학습을 지속적으로 진행하며 추론을 진행할 수 있는 웹 프로젝트입니다


- System Architecture

![SystemArchitecture](./img/sa.png)

AWS EC2에서 S3에 있는 모델과 학습 데이터를 불러와 파인 튜닝을 진행하고 성능이 향상된 모델을 다운하거나 S3에 다시 업로드하여 지속적인 관리가 가능한 시스템입니다.

- Database

![ERD](./img/erd.png)

각 모델의 Task, Metric, 크기, 학습 날짜 등은 1:1 맵핑이 되므로 
별도의 테이블을 생성할 필요가 없었습니다. 따라서 Single table로 모델의 정보를 관리하였습니다.

- Functionality

![page_data](./img/page_data.png)

학습, 추론, 추론 결과 데이터를 관리하는 페이지입니다.

![page_data](./img/page_train.png)

모델을 Matric을 설정하여 학습할 수 있습니다.

![page_data](./img/page_inference.png)

모델을 통해 Inference를 진행합니다. 결과 파일은 S3에 업로드됩니다.

![page_data](./img/page_model.png)

모델 학습 이력을 관리하는 페이지입니다.

</br>

## Installation
### Clone
``` bash
$ git clone https://github.com/c-jinwoo/collab_project.git
$ cd collab_project
```
### Requirements
``` bash
$ pip install -r requirements.txt
```

## Stacks

### Environment
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=Visual%20Studio%20Code&logoColor=white)
![Atom](https://img.shields.io/badge/atom-66595C?style=for-the-badge&logo=atom&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white)
![Github](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white)

### Framework
![Django](https://img.shields.io/badge/django-092E20?style=for-the-badge&logo=django&logoColor=white)

### Development
![HTML](https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white)
![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Machine Learning
![PyTorch](https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Google Colab](https://img.shields.io/badge/googlecolab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

### Cloud
![PyTorch](https://img.shields.io/badge/amazonaws-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)

### Communication
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white)
![Zoom](https://img.shields.io/badge/zoom-2D8CFF?style=for-the-badge&logo=zoom%20Meet&logoColor=white)
