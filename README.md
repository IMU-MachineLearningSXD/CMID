Chinese Medical Intent Dataset(CMID)
====

This dataset is used for Chinese medical QA intent understanding task.


Dataset format:
======
All the data is stored in a JSON file. There are 5 fields in the file. An example as follows:

    {
     "originalText": "间质性肺炎的症状?", 
     "entities": [{"label_type": "疾病和诊断", "start_pos": 0, "end_pos": 5}], 
     "seg_result": ["间质性肺炎", "的", "症状", "?"], 
     "label_4class": ["病症"], 
     "label_36class": ["临床表现"]
    }

The JSON field details
-------
The "originalText" field holds the input information.

The "entities" field holds the Named entity recognition information with Deep learning model. The tag of the entity follows the CCKS2019 Task1 standard: https://www.biendata.com/competition/ccks_2019_1/Evaluation/.

The "seg_result" field holds the information after sentence segmentation.

The "label_4class" field holds the manually annotated medical intent classification information.

The "label_36class" field holds the manually annotated medical intent classification information.

Inclusion of 4class and 36class
-------
label_4class is the primary type that contains: 

    病症 药物 治疗方案 其他

label_36class is the secondary type that contains:

    病症：定义，病因，临床表现，相关病症，治疗方法，推荐医院，预防，所属科室，禁忌，传染性，治愈率，严重性
    药物：作用，适用症，价钱，药物禁忌，用法，副作用，成分
    治疗方案：方法，费用，有效时间，临床意义/检查目的，治疗时间，疗效，恢复时间，正常指标，化验/体检方案，恢复
    其他：设备用法，多问，养生，整容，两性，对比，无法确定

Final Words
======
Thanks for using our corpus! Please don't forget to let us know if our dataset advance the current state of the art forward in your Chinese natural language processing task.

Contacts
======
CMID cannot be used for projects other than scientific research. 

Please contact us if necessary: cssxd@imu.edu.cn
    



