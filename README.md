#

.
├── 상품정보_샘플                            # model directory
│   ├── 무신사_크롤링데이터_샘플                               # checkpoint path
│   │   └── 20_checkpoint_best_regular.pth  # checkpoint file (Download from Google Drive)
│   ├── config                              # config files
│   │   └── DINO
│   │       └── DINO_4scale.py              # Base model config
│   ├── datasets                            # dataset transform/augmentation codes
│   ├── dino_views.py                       # json model output for django server
│   ├── engine.py                           # train/test/eval code for main.py
│   ├── main.py                             # model execute code
│   ├── models                              # model train codes
│   ├── requirements.txt                    # required modules
│   ├── scripts                             # train/eval shell scripts
│   └── util                                # useful codes
│       ├── 20class_plant_coco_id2name.json # id-class matching json file
│       └── visualizer.py                   # make visualized output for dino_views.py
│ 
├── dino_django                             # django api server
│   ├── dino                                # dino model app
│   ├── dino_django                         # django setting
│   └── manage.py                           # run server
│ 
└── extension                               # chrome extension
    ├── dogam                               # 도감 html+js+css+..
    ├── templates                           # 상세정보 html+js+css+..
    ├── xray                                # xray 화면 html+js+css+..
    ├── background.js                       # communicate with django api server
    ├── page.js                             # edit youtube html
    ├── manifest.json                       # chrome extension settings
    ├── newicon-128.png
    └── newicon.png                         # extension icons

