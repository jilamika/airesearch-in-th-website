---
title: Thai Speech Emotion Dataset
description: ชุดข้อมูลจำแนกอารมณ์จากเสียงพูดภาษาไทย
version: 0.8
items:
  - item: Download on GitHub
    description: THAI SER
    size: ~9.85G
    href: https://github.com/vistec-AI/dataset-releases/releases/tag/v0.8
date: "4 March 2021"
featured: true
categories: dataset
image: "/assets/img/releases/speech_emotion_dataset/microphone.jpg"
---

ชุดข้อมูลจำแนกอารมณ์จากเสียงพูดภาษาไทย (Thai Speech Emotion Dataset) ประกอบไปด้วยเสียงพูดภาษาไทยที่สื่ออารมณ์ทั้งหมด 5 อารมณ์ ได้แก่ โกรธ เศร้า สุข หงุดหงิด ปกติ โดยนักแสดง 200 คน (ชาย 87 และหญิง 113) จำนวน 36 ชม. (23,797 ประโยค) พัฒนาโดยสถาบันวิจัยปัญญาประดิษฐ์ประเทศไทย (AIResearch) ร่วมมือกับภาควิชาวิศวกรรมคอมพิวเตอร์ คณะวิศวกรรมศาสตร์ และ ภาควิชาศิลปการละคร คณะอักษรศาสตร์ จุฬาลงกรณ์มหาวิทยาลัย พร้อมทั้งได้รับการสนับสนุนโดยบริษัท แอดวานซ์ อินโฟร์ เซอร์วิส จำกัด (AIS)

ในปัจจุบันมีชุดข้อมูลจำแนกอารมณ์จากเสียงพูดในภาษาต่างๆอยู่ค่อนข้างจำกัด ไม่ว่าจะเป็นภาษาอังกฤษ เยอรมัน อิตาเลี่ยน และอื่นๆ ดังตัวอย่างในตารางที่ 1 แต่สำหรับข้อมูลภาษาไทยยังไม่มีงานวิจัยที่พัฒนาชุดข้อมูลนี้ขึ้นมา ชุดข้อมูลนี้จึงเป็นชุดข้อมูลแรกที่วิจัยในภาษาไทย โดยมีวัตถุประสงค์เพื่อใช้ในการพัฒนาโมเดลการรู้จำอารมณ์จากเสียงพูด และเพื่อนำโมเดลไปประยุกต์ใช้ในอุปกรณ์หรือแอปพลิเคชั่นต่างๆ

|                 ชุดข้อมูล                  |                       ภาษา                        | ชั่วโมง | ประโยค | นักแสดง |                                    อารมณ์                                     |
| :----------------------------------------: | :-----------------------------------------------: | :-----: | :----: | :-----: | :---------------------------------------------------------------------------: |
|     IEMOCAP <br />[Busso et al., 2008]     |                      อังกฤษ                       |   12    | 10,039 |   10    |           โกรธ เศร้า สุข หงุดหงิด ปกติ ตื่นเต้น กลัว รังเกียจ อื่นๆ           |
|   Emo-DB <br />[Burkhardt et al., 2005]    |                      เยอรมัน                      |    -    |  500   |   10    |                   โกรธ เศร้า สุข เซ็ง เครียด กลัว รังเกียจ                    |
|      CREMA-D <br />[Cao et al., 2014]      |                      อังกฤษ                       |    -    | 7,356  |   91    |                       โกรธ เศร้า สุข รังเกียจ กลัว ปกติ                       |
|   EMOVO <br />[Costantini et al., 2014]    |                    อิตาเลี่ยน                     |    -    |  500   |    6    |                    โกรธ เศร้า ตกใจ สุข รังเกียจ กลัว ปกติ                     |
|    MSP-IMPROV<br />[Busso et al., 2016]    |                      อังกฤษ                       |    9    | 7,818  |   12    |                       โกรธ เศร้า สุข รังเกียจ กลัว ปกติ                       |
| DEMoS<br />[Parada-Cabaleiro et al., 2019] |                    อิตาเลี่ยน                     |    -    | 9,697  |   68    |                      โกรธ เศร้า สุข ตกใจ กลัว รู้สึกผิด                       |
|     SEWA<br />[Kossaifi et al., 2019]      | อังกฤษ, จีน, เยอรมัน, กรีก, ฮังการี, และเซอร์เบีย |   44    |   -    |   398   | อารมณ์แบบค่าต่อเนื่อง <br /> (ค่าความสุข: Valence และค่าความตื่นตัว: Arousal) |
|              THAI SER dataset              |                        ไทย                        |   36    | 23,797 |   200   |                         โกรธ เศร้า สุข หงุดหงิด ปกติ                          |

<p style="text-align: center">ตารางที่ 1: ตัวอย่างชุดข้อมูลจำแนกอารมณ์จากเสียงพูดในปัจจุบัน</p>

## รูปแบบการบันทึกข้อมูล

ชุดข้อมูลนี้ประกอบด้วยการบันทึกข้อมูลจำนวน 100 ชุด แบ่งออกเป็น 2 รูปแบบ ได้แก่ การบันทึกข้อมูลในสตูดิโอ (Studio recording) จำนวน 80 ชุด และการบันทึกข้อมูลทางอินเทอร์เน็ต (Zoom recording) จำนวน 20 ชุด

### รูปแบบที่ 1: การบันทึกข้อมูลในสตูดิโอ (Studio recording)

การบันทึกข้อมูลในห้องที่มีสภาพแวดล้อมที่แตกต่างกัน 2 ห้อง ได้แก่ ห้องอัดเสียงระดับมืออาชีพและห้องสำหรับใช้งานทั่วไป พร้อมอุปกรณ์คุณภาพสำหรับบันทึกเสียง ได้แก่ ไมค์คอนเดนเซอร์, ไมค์หนีบปกเสื้อ และกล้องดิจิตอล อุปกรณ์สำหรับบันทึกเสียงและวิดีโอ ตำแหน่งนักแสดงและการวางอุปกรณ์แสดงในรูปที่ 1. การบันทึกข้อมูลรูปแบบที่ 1 ทั้งหมด ถูกจัดทำขึ้นที่คณะอักษรศาสตร์ จุฬาลงกรณ์มหาวิทยาลัย

![studio_setup](/assets/img/releases/speech_emotion_dataset/studio_setup.png)

<p style="text-align: center">รูปที่ 1: ตำแหน่งนักแสดงและอุปกรณ์</p>

### รูปแบบที่ 2: การบันทึกข้อมูลทางอินเทอร์เน็ต (Zoom recording)

การบันทึกข้อมูลผ่านทางเครือข่ายอินเทอร์เน็ต ด้วยโปรแกรม Zencastr สำหรับบันทึกเสียง และ Zoom สำหรับบันทึกวิดีโอ นักแสดงมีอิสระในการบันทึกข้อมูลจากสถานที่, ใช้ไมโครโฟนและกล้องเว็บแคม (webcam) ของตนเอง โดยไม่มีข้อจำกัดของอุปกรณ์

## ขั้นตอนการบันทึกข้อมูล

การบันทึกข้อมูล 1 ชุด จะถูกแบ่งออกเป็น 2 ส่วน

### ส่วนที่ 1: การแสดงแบบมีประโยคให้ (Sentence)

ส่วนนี้จะบันทึกข้อมูลนักแสดงทีละ 1 คน นักแสดงจะต้องพูดตามประโยคที่กำหนดให้ทั้งหมด 3 ประโยค โดย 1 ประโยคจะแสดงทั้งหมด 5 อารมณ์ อารมณ์ละ 2 ระดับคือ ระดับปกติและระดับเข้มข้น ประโยคละ 2 รอบ นักแสดงจะต้องพูดประโยคอย่างถูกต้องและเป็นธรรมชาติ ห้ามเติมคำหรือเปลี่ยนคำในประโยคเด็ดขาด ประโยคที่ใช้ในการบันทึกเสียงได้แก่

    ประโยคที่ 1: พรุ่งนี้มันวันหยุดราชการนะรู้รึยัง หยุดยาวด้วย
    ประโยคที่ 2: อ่านหนังสือพิมพ์วันนี้รึยัง รู้มั้ยเรื่องนั้นกลายเป็นข่าวใหญ่ไปแล้ว
    ประโยคที่ 3: ก่อนหน้านี้ก็ยังเห็นทำตัวปกติดี ใครจะไปรู้ล่ะว่าเค้าคิดแบบนั้น

### ส่วนที่ 2: การแสดงแบบกำหนดสถานการณ์ (Improvisation)

ส่วนนี้จะบันทึกข้อมูลนักแสดงเป็นคู่ นักแสดงแต่ละคนจะได้รับบทบาทที่แตกต่างกัน (บทบาท A และ บทบาท B) ตามสถานการณ์ที่กำหนดไว้ นักแสดงแต่ละคู่จะต้องสนทนาตามบทบาทและอารมณ์ที่กำหนดให้ทั้งหมด 5 สถานการณ์ แต่ละสถานการณ์จะต้องแสดงยาวต่อเนื่องประมาณ 3 นาที และจะบันทึกสถานการณ์เพียงหนึ่งครั้งเท่านั้น สถานการณ์ทั้งหมดแสดงตามตารางที่ 1 ด้านล่าง

| สถานการณ์ | บทบาท A                                                                                 | บทบาท B                                                                                  |
| :-------: | --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
|     1     | พนักงานฝ่ายต้อนรับในโรงเเรมที่พยายามรับมือและไกล่เกลี่ยกับลูกค้าที่ไม่พอใจ (ปกติ)       | ลูกค้าที่ไม่พอใจโรงแรมหรือบริการบางอย่างของโรงแรม เลยต้องการเรียกร้องหรือตำหนิ (โกรธ)    |
|     2     | เพื่อนที่มาบอกข่าวดีว่าจะแต่งงาน และต้องการชวนคู่สนทนา ไปงานแต่งและช่วยในงานเเต่ง (สุข) | เพื่อนที่ได้รับข่าวดี ร่วมยินดีและตื่นเต้นกับการที่จะได้ช่วยคิดงาน (สุข)                 |
|     3     | คนไข้ที่มาปรึกษาอาการป่วยและระบายปัญหาชีวิต (เศร้า)                                     | หมอที่รับฟังปัญหาหรืออาการป่วยของคนไข้ (ปกติ)                                            |
|     4     | เจ้านายหรือรุ่นพี่ที่ต้องการต่อว่าคู่สนทนา เรื่องการทำงาน (โกรธ)                        | ลูกน้องหรือรุ่นน้องที่โดนคู่สนทนาที่ตัวเองไม่เคารพต่อว่า และรู้สึกว่าตัวเองไม่ผิด (เซ็ง) |
|     5     | เพื่อนหรือพี่น้องที่บ่นเกี่ยวกับพฤติกรรมบางอย่างที่ตัวเองรู้สึกไม่พอใจ (เซ็ง)           | เพื่อนหรือพี่น้องที่โดนบ่นแล้วรู้สึกผิด และพยายามขอให้อีกฝ่ายยกโทษให้ (เศร้า)            |
|     6     | พนักงานในโรงเเรมที่มีใจรักในการบริการ ที่พร้อมจะทำทุกอย่างให้ลูกค้าพอใจ (สุข)           | ลูกค้าที่มาเข้าพักในโรงแรม ที่รู้สึกพอใจในโรงแรมและการบริการเป็นอย่างมาก (สุข)           |
|     7     | คนที่กำลังจะเเต่งงาน แต่ไม่มั่นใจว่าควรแต่งหรือไม่ แต่ก็ไม่กล้าปฏิเสธการเศร้า (เศร้า)   | คนรับฟังปัญหาและเริ่มรำคาญ เพราะฟังมาบ่อยมากแล้ว และแนะนำอะไรไปก็ไม่ฟัง (เซ็ง)           |
|     8     | คนไข้ที่มาปรึกษาอาการป่วยและมีเรื่องรำคาญใจ (เซ็ง)                                      | หมอที่รับฟังปัญหาหรืออาการป่วยของคนไข้ (ปกติ)                                            |
|     9     | พนักงานฝ่ายทรัพยากรบุคคลที่ได้รับมอบหมายให้มาแจ้งพนักงานเรื่องการเลิกจ้าง (ปกติ)        | พนักงานที่โดนเลิกจ้าง ที่ไม่อยากถูกเลิกจ้างด้วยเหตุผลส่วนตัว (เศร้า)                     |
|    10     | คนที่โกรธที่อีกคนทำผิดอะไรมาสักอย่าง (โกรธ)                                             | คนที่โมโหที่อีกคนมากล่าวโทษและต่อว่าอย่างรุนแรง (โกรธ)                                   |
|    11     | ผู้กำกับที่เบื่อและเซ็ง เพราะยังไม่ได้อย่างที่ต้องการ (เซ็ง)                            | นักแสดงหรือทีมงาน ที่ทำให้แล้วแต่ยังไม่ถูกใจสักที (เซ็ง)                                 |
|    12     | คนที่ได้ย้ายไปทำงานใหม่/ตำแหน่งใหม่ในต่างประเทศ ที่มาเล่าให้เพื่อนฟัง (สุข)             | คนที่รู้สึกว่าตัวเองยังอยู่ที่เดิมและเศร้าที่ เพื่อนจะจากไปไกล (เศร้า)                   |
|    13     | คนไข้ที่ไม่เข้าใจโรคหรือวิธีการรักษา และสอบถามข้อมูลหมอ (ปกติ)                          | หมอที่ตรวจคนไข้แบบใจดี และพยายามอธิบายวิธีการรักษา (สุข)                                 |
|    14     | พนักงานที่โมโหลูกค้าหรือหัวหน้า แล้วมาเล่าให้เพื่อนฟัง (โกรธ)                           | เพื่อนที่รับฟังเรื่องราวของเพื่อน (ปกติ)                                                 |
|    15     | คนที่โดนแฟนนอกใจ และรู้สึกเสียใจที่โดนหลอก (เศร้า)                                      | เพื่อนที่ฟังเรื่องของเพื่อแล้วรู้สึกโมโหในสิ่งที่เพื่อนต้องโดน (โกรธ)                    |

<p style="text-align: center">ตารางที่ 2: สถานการณ์ บทบาทและอารมณ์ที่กำหนดในการแสดง</p>

## การระบุอารมณ์จากเสียงพูด

หลังจากบันทึกข้อมูลเรียบร้อยแล้ว ข้อมูลเสียงทั้งหมดจะถูกตัดเป็นประโยคย่อย และนำมาระบุอารมณ์ ด้วยวิธีคราวด์ซอสซิ่ง (crowdsourcing) โดยให้ผู้ประเมินฟังเสียงและเลือกอารมณ์ผ่านระบบ ผู้ฟังสามารถเลือกอารมณ์ที่แสดงให้ 5 อารมณ์ ได้แก่ โกรธ เศร้า สุข หงุดหงิด ปกติ หรือสามารถเลือก ‘อื่นๆ’ ได้ในกรณีที่คิดว่าเป็นอารมณ์อื่น ข้อมูลเสียง 1 ประโยคจะใช้ผู้ประเมินทั้งหมด 3-8 คนและใช้วิธีเสียงข้างมากเพื่อเลือกเป็นอารมณ์สำหรับประโยคนั้นๆ (Majority emotion) และคำนวณค่าความเห็นพ้องของอารมณ์ในประโยค (Majority agreement)

### ความเชื่อมั่นระหว่างผู้ประเมิน (Inter-rater reliability)

ข้อมูลอารมณ์ที่ได้รับจากผู้ประเมินทั้งหมดจะถูกนำมาความเชื่อมั่นระหว่างผู้ประเมิน ซึ่งเป็นการวัดความสอดคล้องภายในคำตอบทั้งหมดระหว่างผู้ประเมินตั้งแต่ 2 คนขึ้นไป ผู้ประเมินแต่ละคนมีความเป็นอิสระต่อกัน โดยใช้หลักการที่ว่าเมื่อผู้ประเมินทำแบบทดลองด้วยแบบชุดเดียวกัน ผลการสังเกตที่ได้ควรจะสอดคล้องกัน ค่าความสอดคล้องจะขึ้นอยู่กับความคงเส้นคงวาของคำตอบของผู้ประเมินในข้อมูลชุดนี้จะใช้วิธีการคำนวณความสอดคล้องระหว่างผู้ประเมินด้วย [Krippendorff’s Alpha](https://en.wikipedia.org/wiki/Krippendorff%27s_alpha) ซึ่งสามารถใช้ได้กับผู้ประเมินจำนวนเท่าใดก็ได้ จำนวนคำตอบของแต่ละข้อไม่เท่ากันได้ และใช้มาตรวัดระยะห่าง (Distance metric) ได้หลากหลาย ในที่นี้ใช้ [Measuring Agreement on Set-values Items (MASI)](https://www.researchgate.net/publication/228528415_Measuring_agreement_on_set-valued_items_MASI_for_semantic_and_pragmatic_annotation) [Passonneau et al. 2006] ค่าของ Krippendorff's alpha มีค่าเท่ากับ 1 แปลว่าข้อมูลชุดนั้นมีความน่าเชื่อเป็นอย่างมาก ในการนำไปใช้ค่า alpha ควรมีค่ามากกว่าหรือเท่ากับ 0.667 ถ้าน้อยกว่านั้นถือว่าคำตอบไม่มีความสอดคล้องกันและไม่น่าเชื่อถือ

เมื่อนำข้อมูลอารมณ์ทั้งหมดมาประเมินค่าความเชื่อมั่นระหว่างผู้ประเมินอยู่ที่ 0.42 ทางผู้พัฒนาถึงทำการคัดเลือกประโยคที่มีค่าความเห็นพ้องของอารมณ์ในประโยคมากกว่าหรือเท่ากับ 0.7 เป็นต้นไป มาคำนวณใหม่ ได้ค่าความเชื่อมั่นอยู่ที่ 0.67 ซึ่งเป็นค่าที่แสดงความความสอดคล้องและน่าเชื่อถือของคำตอบ จำนวนประโยคในแต่ละอารมณ์แสดงในตารางที่ 3

|                   | ข้อมูลอารมณ์ทั้งหมด | ข้อมูลอารมณ์ที่มีค่าความเห็นพ้องของอารมณ์ในประโยคมากกว่าหรือเท่ากับ 0.7 |
| :---------------: | :-----------------: | :---------------------------------------------------------------------: |
|       ปกติ        |        6172         |                                  3791                                   |
|       โกรธ        |        2745         |                                  1880                                   |
|        สุข        |        3594         |                                  2739                                   |
|       เศร้า       |        2356         |                                  1447                                   |
|     หงุดหงิด      |        6614         |                                  3359                                   |
|    อารมณ์อื่นๆ    |          4          |                                    0                                    |
| ไม่มีความเห็นพ้อง |        2239         |                                    0                                    |
|     **Total**     |      **23724**      |                                **13216**                                |

<p style="text-align: center">ตารางที่ 3: เปรียบเทียบจำนวนประโยคในแต่ละอารมณ์ก่อนและหลังคัดเลือกประโยคที่มีค่าความเห็นพ้องของอารมณ์ในประโยคมากกว่าหรือเท่ากับ 0.7</p>

รูปที่ 2 และ 3 แสดง confusion matrix ระหว่างอารมณ์ที่ระบุให้นักแสดงแสดง (Assigned emotion) กับอารมณ์จากเสียงข้างมากของผู้ประเมิน (Majority emotion) ซึ่งจะเห็นได้ว่าอารมณ์ที่ผู้ฟังมีความเห็นตรงกับสิ่งที่นักแสดงต้องการจะสื่อมากที่สุดคืออารมณ์ปกติ (Neutral) ในขณะที่อารมณ์โกรธ (Angry) และอารมณ์เศร้า (Sad) ผู้ฟังมักจะสับสนกับอารมณ์หงุดหงิด (Frustrated)

![CM_all_v1](/assets/img/releases/speech_emotion_dataset/CM_all_v1.png)

<p style="text-align: center">รูปที่ 2: emotion confusion matrix แสดงค่าจากจำนวนประโยคทั้งหมด</p>

![CM_07_v1](/assets/img/releases/speech_emotion_dataset/CM_07_v1.png)

<p style="text-align: center">รูปที่ 3: emotion confusion matrix แสดงค่าหลังจากคัดกรองค่าความเห็นพ้องของอารมณ์ในประโยคมากกว่าหรือเท่ากับ 0.7  (ปกติ: Neutral, โกรธ: Angry, สุข: Happy, เศร้า: Sad, หงุดหงิด: Frustrated, อารมณ์อื่นๆ: Other, ไม่มีความเห็นพ้อง: None)</p>

## อ้างอิง

- Busso, Carlos, et al. "IEMOCAP: Interactive emotional dyadic motion capture database." Language resources and evaluation 42.4 (2008): 335-359.
- Grimm, Michael, Kristian Kroschel, and Shrikanth Narayanan. "The Vera am Mittag German audio-visual emotional speech database." 2008 IEEE international conference on multimedia and expo. IEEE, 2008.
- Busso, Carlos, et al. "MSP-IMPROV: An acted corpus of dyadic interactions to study emotion perception." IEEE Transactions on Affective Computing 8.1 (2016): 67-80.
- Cao, Houwei, et al. "Crema-d: Crowd-sourced emotional multimodal actors dataset." IEEE transactions on affective computing 5.4 (2014): 377-390.
- Kossaifi, Jean, et al. "Sewa db: A rich database for audio-visual emotion and sentiment research in the wild." IEEE transactions on pattern analysis and machine intelligence (2019).
- Costantini, Giovanni, et al. "EMOVO corpus: an Italian emotional speech database." International Conference on Language Resources and Evaluation (LREC 2014). European Language Resources Association (ELRA), 2014.
- Parada-Cabaleiro, Emilia, et al. "DEMoS: An Italian emotional speech corpus." Language Resources and Evaluation (2019): 1-43.
- Passonneau, Rebecca. "Measuring agreement on set-valued items (MASI) for semantic and pragmatic annotation." (2006).
