
[![Jitpack](https://jitpack.io/v/FangStarCom/CallRecord.svg)](https://jitpack.io/#FangStarCom/CallRecord)
[![Build Status](https://travis-ci.org/FangStarCom/CallRecord.svg?branch=master)](https://travis-ci.org/CListery/CallRecord)
[![Min Sdk Version](https://img.shields.io/badge/API-19%2B-blue.svg?style=flat-square)](https://developer.android.com/about/versions/android-4.4.html)
[![License](https://img.shields.io/badge/License-Apache%20License%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)

# CallRecord
通话记录同步记录库

## 工作原理
1. 该库通过 PhoneStateListener 监听当前通话记录并且兼容至 Android KitKat
2. 在某些低版本机型无法通过 PhoneStateListener 的回调获取到当前通话号码，则在通话结束后通过时间范围锁定目标系统通话记录并同步数据
3. 使用 MediaRecorder 对 VOICE_COMMUNICATION 进行监听并输出为音频 (由于无法直接监听通话上下流，所以音频质量较差，目前该功能比较鸡肋)

## License
   Copyright [2019] clistery <cai1083088795@gmail.com>

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at
   
       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
   
## Dependencies
- [Realm](httpshttps://github.com/realm)
- [RxAndroid](https://github.com/ReactiveX/RxAndroid)
- [Kotlin-Realm-Extensions](https://github.com/vicpinm/Kotlin-Realm-Extensions)
- [Timber](https://github.com/JakeWharton/timber)
- [AndLinker](https://github.com/codezjx/AndLinker)
