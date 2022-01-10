# cse608-assignments
* Assignment 1 [planetuml link](http://www.plantuml.com/plantuml/uml/VPBTxjiW3CNlUGghztc5gLkhIPCsQLgxwya19qKZWB3fb7sy-o2XQNFplygn_JkAEN1amIHvSihH8201aXrl0iOcqcA3LmgrX0JVcH8WGoxVH-_aB7cfNUsKYgX_uaXm4Ho6skGg_YY0bJvyJS5aBV05VU7IeJBJDZuJsz6lFp5FqpN4DceE2V5bVCeiOIgk2wMxrRGWcf_0XyniFJ43UdGpoqBqgFvj2r_3_76XPwZRPYQDJ73u74Rh5pp_S5Mhr-abzvCLY2d4mEWQnt47dUdkGhH-1BbHOybK8K7cICrbzgvlTBVqwsrBsbjAjjbe0f0mSqEYx91FNYYX5a1lO2I1WSZq9OE6ZyCEVr_Z-atGvpM_Hc5Ve1BUShdGrLVJ_NstFWljeCjnArMzAkXgRPIghL9iMHPwBJbkigoWUPCFVmkeoNggQPKbWnvNMTOwaZTvSly1) 
* Assignment1 [online word report](https://engasuedu-my.sharepoint.com/:w:/g/personal/2101398_eng_asu_edu_eg/EW6_-ZXMwapFrVV4nNACJHMBJjRv74BawB33d8nUSPfVcA?e=F5bwLm)

# Assignment 1 Description  (Thanks to ALLAH)[DONE]
A factory produces kids toys. the process of production depending on **getting a proposal** and **developing a prototype** and finally **produce the toys** and **getting feedback from the client**. **a top designer do the proposed prototype**. that usually **reviewed by a product manager**. **The business of the factory business needs to be automated** and also **the amount of sales and feedback related to toys needs analysis** and **Business analytics**.

* The toy factory has:
1. number of toy designers. 
2. product managers.
3. customer service who interact with client to propose toys and get feedback.

## Requirements:
1. create a detailed USE case diagram and make all possible assumptions

2. write the detailed use case description for two use cases 

3. create a at least 10 INVEST user stories, and put them in a diagram value-vs-difficulty

* **provide neat diagrams and make reasonable assumptions**

4. work in a team of two or individuals.

## Project State Diagram


```mermaid
stateDiagram
    [*] --> Proposal
    Proposal --> PrototypeDevelopment
    PrototypeDevelopment--> ManagerReview
    ManagerReview --> PrototypeRework
    ManagerReview --> ClientReview
    PrototypeRework --> ManagerReview
    ClientReview --> MassProduction
    ClientReview --> PrototypeRework
    MassProduction--> [*]
```

![Project State Diagram](diagrams/project-state-diagram.png**


# Assignment 2
## [Usecases link](http://www.plantuml.com/plantuml/uml/RLDDZnCn3BtdLrYzSEe_uB2m8420X8IMQ-LDt3HgFaQnGwc0_yuaqybEbZsCb7b-By-oN-vOC4i9Ndaw2aY2xEn9mBXCMboAIg6MbE61AGCo5AQi9jHdj0IxTyYdnvJHj3hlAiFC6FnM08jmzrsAeIYjnilvgNYVIcQ2Jv4bbmerckk_cskkB1JWZGakDXBMa_ghUZVlJVc0WPftOTB81BiloS9DK0u-sLcYjlNgZDw3d0YMPbunM0nqapXjVnrug_ZcyLhfMzPaHyuFHnS8LvXoifcORxIVuIMUNcOGK2Wxz9siUIH_ZgbT6XmBdcdbdKCOUMy9yD5JNUQ4CmeOpMmInSL2_tMkQqjR-SDaK1OEiA3jHiNomMsPNrDqTJUPk7XXICTrmQiavFHCSvz2AD7fQd5nSdgkq9Sg65pGHPa_u2K1nn9RCj4xkQu-V3pWLlGHe_446Az0EQVS8eLH_Aeu8Ra3LYC5DKGrr_3wpxvC-vRW6xBVRs9pQxM2FHW3Dja1wHiV8SqZr7UumVfYrDDRcF6-XH7jWnxXFatLtieCzL5re4_YZg8fmVy3)

## [Sequence dashboard link](http://www.plantuml.com/plantuml/uml/bPNFRjim3CRlUWeYEzH9czDk0JPqQzTXXs85zkSo384Iivu6MJ8akKNozBCeQvEL1jPoQMrzdqZ-J57Nrd7Z-bOotZkj-dQ7Xh4BU4K_44eu8RauSYUq0lq8xXT2gskKNa8_nXQRZxp51yaFQ1O0wxS0uTLtWSyBkBpS08NnhwebIzQyDZpUQEMCbdBO8TSpbal8bqRzf1ur-HfqDxetTX3N52iNmVgbaElr1lRas-u7u_cGjzpn3n9RL2x6-xpxZNjNXJzV3ns-kGXRNLobUoxPn9tij-CMusQaGEaLbUBjp5xaX7MUMLgEfhHUZ1r0BM2r6jG6kSEn59SMaUKz3p14F8ymX8q5Vt6yYN6NBAwUfnFp84jaPFqc0w8V2QChUad__Zpb5GDHugICUSVc3qY4Qa3XCuH5g5Qh9RJ8bHs9qM8y24ds589gI_bEYytrEQxJr799OgJpH9OTDa9jduR7RSqTPzFpbXqSSZJ3Ox1Pzg_-RX3uydb88bRf1VIBBo0K0IrtQ0INTbp8ne8Fd0s5bYlidz0KpWMO7F3xCLpIEuHtla5ZeX5h4TNSkzFaBMCR2_Ku3QeQ3TQCvIIXwuz7IQ3B-D6Gt9BhV_WzaA6SsvXNEQxSCayfo1CsaSo4ZzNooIDCE14egNK7hy5HzsMgMOgany2auie-evb7EMCycNb15Mp2tcXZFFjeujBvpNgwOuM5VLXd012zvpuFU7e7jAGjkoOttxhQpw8X2bRZTnBradR8nVaSXerrtiQbyz-91ioIeRG8pXo0Dq91STfAatIsdqWSMgEQz5MQStbpaOaD3oVdxuuBYRNl9D6Y1Q4cdSOQe_iE7YSYLexzlfTET0VY_lvmYtiQhtTyFn3DlaDgBli4HHmt1cbaq7aVJluSl75wZIwi2ThvYvssZLVrEsj5e_nDROjc3F-hZqEZA4peija8S3gJheTY-bR-0G00)


## [Sequence game link](http://www.plantuml.com/plantuml/uml/bPNFRjim3CRlUWeYFJH9czDk0JPqQzTXXs85zkSo384Iivu6MJ8akKNwz9EeQ9EL1bPzIMnzdqZ-JD5Nrd7ZXauoFZYjXcwBXh5pEACBX19EI2wUkHDQWNu0znkXqmrAaeIBiTdw4-_mNl8zcXd0wXr0VFH3uDCCBYxMG672e_c2vMjU6s-ljN96I-btAFMCbHBovL4_gmTDlXRTjHwCzUA6OfKYMBqKShLQmuvycvqtdWvvmnt_AB53vLAyBzi_k7Fp-FDjt-FRyxZL-MM-vuADtDb-MsunRKOAb44nLxoRs8kSi2epoylHbDQBiIEe6IoNNcsGEpoKul8YYhod0SQ8fn76iAdWhuwtAUw2fTNJT58UP4cChDya8FgPCRgaX_Jtrp6l58WI9sNAEpL_H29K2mgV82x2VBbSG8TSsRYCj7WMhpnx2a6rvNp7nPRwOwPbQgKaCz9v8iiMMw4sZ_vsqt37sVYy5GU77As_ZJRB_jVVUq4edySaKfL1G5Tw0B48wBX38xYqXuLYBFZ0vL3ekCBX4KtbN83H0RyxXCjwX_1EDsXAD66jebfwjvgyTMnJeG6dGTMWmOQnaYJqm_Ep9D1r_6X8RiZr6dxtP7W5jnYX7bTfcQOKvHcRH6R4nshvw14MdCwOrBg7D-2e-mhL94NIOsGovye-ePb4EM4yddbH5Mt2NcjZ0ljaujA5pGRwnWeBkxZE021vJxqU2FJsQ4bRzvbSV--RC8jy59mVtfDe5hH3AIxdCAoj2pQVSNXFD60M3AL5JtyFl1KAgjDMcgIJ_KJYs1hpKL_bETSt5vcOlpawVxTSI6n29uaEBGWrwZJM6Ztqy30IiNhiTuDqejyJzm_x6zpHUBtbEq-qU0-vkUuLL75S6wIHGUVTd_mfU8VfTN1XGz08tAa-fvtJr_gzjQ9LuMDjgyOC_wTFSwCgJ6oqoGXmF9QkV2r39_y2)


###[]
**It is required to build a software application in one of the following domains:**

## 3. Virtual Reality Educational Game
* Virtual Reality Educational game based on topics from one course,
* students have **levels** 
* The course is divided into stages 
* Each student must complete all stages before he proceed to the final stage
* The course stages can be edited and updated by course instructors

## Team members
In teams of 1/2/3 create the following

## Requirements

1. userstories
2. functional and non functional requirements 
3. list all stakeholders
4. use case diagram
4. provide use case description for at least **two use cases**
5. create all required development uml models like:
* class diagram 
* time sequence diagram 
* state diagram
6. provide short research about the main system users UX 
* and design at least two UI screens

## What to hand
1. A word document containing all text diagrams, models and 
2. A presentation in ppt.pptx similar to the library case study
3. Possibly use draw.io for your **diagrams either copy and past or have link for the diagram in your word document**
