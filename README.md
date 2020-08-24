# Dumbpad x VIA Configurator

(中文在下方)

Dumbpad With VIA Configurator

## Dumbpad

[Dumbpad](https://github.com/imchipwood/dumbpad)

## VIA Configurator

[VIA Configurator](https://caniusevia.com/) is a online configurator tool, it can change your keyboard layout realtime. No need to recompile or reflash the firmware.

But if you want some functions like, Encoder, User space, code. It can't help you.

## Dumbpad X VIA Configurator

### Enable VIA (QMK)

Add the setting in your `rules.mk`, create it if doesn't exist.

> VIA_ENABLE = yes

### Setup your encoder KEYCODE
The VIA Configurator doesn't support encoder, so you need to setup it before you flash the firmware.
I already create few different firemware for encoder function, like MOUSE UP/DOWN, VOLUME UP/DOWN, PAGE UP/DOWN.
If this fit your demand, you can donwload it and flash to the controllers. The simlpy way is using QMK Toolbox.
I will contribute firmware and json to QMK and VIA, During the time, you need to download the json file and import into VIA Configurator.

### Import JSON to VIA Configurator

Please download via_configurator_json/dumbpad_via.json to your local.

- Launch VIA Configurator.
- Switch to tab "**SETTINGS**".
- Enable "**Show Design tab**" then you can see "DESIGN" tab in the top.
- Switch to tab "**DESIGN**".
- Click on "**Load**" and select the json file.
- Switch to "**CONFIGURE**" and plug-in your Dumbpad.

# 如何使用 VIA Configurator 設定 Dumbpad

使用 VIA Configurator 設定 Dumbpad

## Dumbpad

[Dumbpad](https://github.com/imchipwood/dumbpad) 是 4x4+1 的小鍵盤，並且有一個旋鈕可以旋轉，旋鈕本身可以下壓，所以也是一個按鈕。

## VIA Configurator

[VIA Configurator](https://caniusevia.com/) 是可以即時編輯鍵盤配置的軟體，需要安裝，使用 VIA 就不須要在修改鍵盤配置的時候重新燒錄韌體，可以免去許多麻煩。

但有些功能 VIA 無法支援，例如旋鈕旋轉的動作，或是您要自訂 User Space 的動作。

## Dumbpad 與 VIA Configurator

### 在 QMK 中啟用 VIA

Add the setting in your `rules.mk`, create it if doesn't exist.

請先開啟 QMK 韌體，並在 `rules.mk` 中加入下列的設定，如果檔案不存在的直接建立即可。

> VIA_ENABLE = yes

### 設定旋鈕的鍵盤代碼
目前 VIA Configurator 不支援旋鈕，只能修改鍵盤的功能，所以您必須在燒錄之前就設定好旋鈕。
我已經先準備了幾個韌體，針對旋鈕設定了不同的功能，例如滑鼠滾輪上/下、音量增/減、上一頁/下一頁。
如果這些韌體剛好是您需要的，可以直接下載燒錄即可。使用 QMK Toolbox 燒錄是最簡單的方式。
我將會正式推送到 QMK firmware 與 VIA Configurator，但在此之前，您可以直接下載後燒錄。

### 載入設定檔 (JSON) 到 VIA Configurator 

請下載 via_configurator_json/dumbpad_via.json 到您的電腦。

- 執行 VIA
- 切換到 "**SETTINGS**" 分頁
- 啟用  "**Show Design Tab**"，就可以看到 "DESIGN" 分頁
- 切換到 "**DESIGN**" 分頁
- 按下 "**Load**" 並選擇 "**dumbpad_via.json**"
- 切換到 "**CONFIGURE**" 分頁並且接上您的 Dumbpad 就可以開始編輯鍵盤配置。

Author: HaWay, Contributed by [ErgoTaiwan](https://ergotaiwan.com)

