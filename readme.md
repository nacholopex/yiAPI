Hi👋🏼 everyone.
I was requesting some type of access to the API or something similar to create new features to `yitechnology.com`, but I didn't get any response in the pasts months.
So I was spending my free time knowing how the YiHome App works.

# Login to the account
GET --> `https://gw-us.xiaoyi.com/v4/users/login?seq=1&account=USER@EMAIL.COM&password=xxxxxxxxx`
```json
{
    "code":"2000",
    "data":{
        "birthday":"Birthday 🎂",
        "img":"http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/userfiles/USERID/profile_img_XXXX.jpg?Expires=XXXX&OSSAccessKeyId=XXXXXXXX&Signature=XXXXXXXX",
        "flag":true,
        "mobile":"",
        "last_name":"",
        "userid":"00000",
        "register_time":"Unix Time Stamp",
        "token":"32 characters",
        "token_secret":"32 characters",
        "name":"YI_XXXXX",
        "first_name":"",
        "account":"user@email.com",
        "email":"user@email.com"
    }
}
```

# Promotional things inside APP
GET --> `https://gw-us.xiaoyi.com/v5/app/config?location=US&language=es-ES`
```json
{
    "code": "20000",
    "data": {
        "adsUrl": {},
        "cloud_storage": {
            "images": [
                {
                    "index": 0,
                    "url": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/1-1080p_cloudstorage.png"
                },
                {
                    "index": 1,
                    "url": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/2-encryption2.png"
                },
                {
                    "index": 2,
                    "url": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/3-all_weather.png"
                },
                {
                    "index": 3,
                    "url": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/4-people_counting.png"
                }
            ],
            "kami_price_link": "https://api.yitechnology.com/homecamera/yi_cloud_price_plans_ios.html",
            "price_link": "https://api.yitechnology.com/homecamera/yi_cloud_price_plans.html",
            "iapprice_link": "https://api.yitechnology.com/homecamera/yi_cloud_price_plans_ios.html",
            "kami_iapprice_link": "https://api.yitechnology.com/homecamera/yi_cloud_price_plans.html"
        },
        "newFeature": false,
        "pcViewTimeP2P": "1800",
        "help_video": {
            "help_video_en-US": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/help/YiHome_Pairing_Tutorial_en_US.mp4",
            "help_video_zh-TW": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/YiSmart-Connect-tutorial-zh-TW.mp4",
            "help_video_ko-KR": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/YiSmart-Connect-tutorial-ko-KR.mp4",
            "help_video_zh-CN": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/help/YiHome_Pairing_Tutorial_zh_CN.mp4"
        },
        "userAgreement": {
            "userAgreementVersion": "1.1",
            "userAgreementUrl": "http://api.yitechnology.com/home/terms_of_use?location=USA&lang=es-ES",
            "userPrivacyUrl": "http://api.yitechnology.com/home/privacy_agreement?location=USA&lang=es-ES"
        },
        "pcViewTimeRelay": "1800",
        "cloudstorage_intro_video": {
            "cloud_intro_video_en-US": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/gesture/YiHomeCamera_CloudStorage_Tutorial_en_us.mp4"
        },
        "3rdparty_ads": {
            "adChannel": "yi",
            "distribution": {
                "mi": 0,
                "tencent": 0
            }
        },
        "bindSwitch": "0",
        "kami_app_cloud_disable": "0",
        "is_iapautorenew_dogfooduser": "0",
        "disableNonMiBind": "0",
        "iap_renew_switch": "1",
        "app_alert_oneday_utc_starttime": "1595991600000",
        "h5productpages": {
            "cloudstorage_product_page_2": "https://clouldh5-us.xiaoyi.com/h5/index.html",
            "cloudstorage_product_page_1": "https://clouldh5-us.xiaoyi.com/newh5/#/tobuy",
            "cloudstorage_product_activity_page": "https://clouldh5-us.xiaoyi.com/newh5/#/tobuy",
            "cloudstorage_iap_product_page_1": "https://clouldh5-us.xiaoyi.com/newh5/#/tobuy",
            "cloudstorage_page_ios_renew": "https://clouldh5-us.xiaoyi.com/h5/kamicloudplans.html",
            "battery_product_buy_page": ""
        },
        "gesture_video": {
            "gesture_video_en-US": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/gesture/YiHomeCamera_Gesture_Tutorial_en_us.mp4",
            "gesture_video_zh-TW": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/gesture/YiHomeCamera_Gesture_Tutorial_zh_cn.mp4",
            "gesture_video_ko-KR": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/gesture/YiHomeCamera_Gesture_Tutorial_en_us.mp4",
            "gesture_video_zh-CN": "http://yihome-publicfiles-us.oss-us-west-1.aliyuncs.com/publicfiles/homecam/gesture/YiHomeCamera_Gesture_Tutorial_zh_cn.mp4"
        },
        "disableNonMiNewAccount": "0",
        "androidUpgrate": {
            "androidLatestVersionMsg": "- New add credit card payment method to subscribe YI Cloud.&&- Fixed bugs, optimized user experience.",
            "androidLatestVersionCode": "72",
            "androidForceVersionCode": "1"
        }
    }
}
```

# Alert list notifications
GET REQUEST --> `https://gw-us.xiaoyi.com/v2/alert/list?fromDB=true&expires=10&sub_type=&hmac=xxxxxxxxxx=&limit=100&from=UNIXTIME&to=UNIXTIME&type=&userid=USERID&seq=0`
```json
{
    "code": "20000",
    "data": [
        {
            "video_pwd": "video_password_unique",
            "pic_urls": "http://motiondetection-us.oss-us-west-1.aliyuncs.com/YEAR/MONTH/DAY/USERID/UID_UNIXTIMESTAMP_0.jpg?Expires=UNIXTIMESTAMP&OSSAccessKeyId=XXXXXX&Signature=XXXXXXXXXXXXX",
            "type": 0,
            "message": "Message to know the camera that has the alert",
            "pic_pwd": "pic_password_unique",
            "uid": "ID of the camera",
            "sub_type": 1,
            "media_type": 0,
            "name": "Alert Event",
            "video_urls": "http://motiondetection-us.oss-us-west-1.aliyuncs.com/YEAR/MONTH/DAY/USERID/UID_UNIXTIMESTAMP_0.mp4?Expires=UNIXTIMESTAMP&OSSAccessKeyId=XXXXXX&Signature=XXXXXXXXXXXXX",
            "id": "Identifier",
            "time": "Unix time stamp",
            "category": 0
        }
    ]
}
```
# Update status firmware specific camera
GET --> `https://api.us.xiaoyi.com/vmanager/upgrade?uid=CAMERA_ID&protocol=mius&sname=familymonitor-y203c&version=FIRMWARE_VERSION`
```json
{
    "code": 20000,
    "needUpdate": "false",
    "multiMessage": " ",
    "forceUpdate": "false",
    "message": " "
}
```

# Device info
GET --> `https://gw-us.xiaoyi.com/v5/devices/deviceinfo?uids=CAMERA_ID&hmac=XXXXXXXXXXXXX&userid=USER_ID&seq=1`
```json
{
    "code": "20000",
    "data": {
        "TNPUSAH-397670-SRZKW": {
            "appParam": {},
            "timezone": "Europe/Paris",
            "model": "6",
            "language": "en-US",
            "did": "6FUSY213EUWV0A190304"
        }
    }
}
```

# Edit camera name
GET --> `https://gw-us.xiaoyi.com/v2/devices/edit?uid=CAMERA_ID-SRZKW&hmac=XXXX&name=NEW_NAME&message=&userid=USER_ID&seq=1&token=TOKEN`
```json
{"code":"20000"}
```