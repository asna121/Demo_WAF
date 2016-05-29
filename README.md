# DEMO WAF with STM32F429I-Discovery

這裡說明有那些Demo資料夾及要如何使用。

## 前期準備

測試環境是*Ubuntu 14.04 LTS* 預先安裝了*WAF*和*ARM-GCC*

- WAF [官網](http://code.google.com/p/waf/) 另外可以去參考，站內底下的連結 *WAF Book* 和 *API DOC* 

- GCC ARM Embedded [官網](http://launchpad.net/gcc-arm-embedded/+download)

到STM官網下載最新的 STM32CubeF4 Package，以及STLINK Driver

- ST [STM32CubeF4](http://www.st.com/content/st_com/en/products/embedded-software/mcus-embedded-software/stm32-embedded-software/stm32cube-embedded-software/stm32cubef4.html) 下載連結在頁面底下，解壓縮後把此檔案與GitHub上的資料夾放在一起。

安裝ST-LINK工具
- HACKPAD [st-link](https://stm32f429.hackpad.com/WbiooOfkaoR_cPHciRtOYRJ#NOTE) 請參考連結操作。
- 其他安裝參考 [st-link](http://startingelectronics.org/tutorials/STM32-microcontrollers/programming-STM32-flash-in-Linux/)

## WAF Command

### How?

把terminal移到想要測試的project底下，在terminal輸入底下指令

### General Command

- `./waf configure` to set the compiler information
- `./waf clean` to clean what I don't know yet
- `./waf program` to activate st-link to load program to STM32F4

## Project List

### LED-Blink
在STM板子上，按下Buttom(藍色)，可以看到LED亮起來，再按一次會熄滅

### LTDC_Display_2Layers
使用STM板子上的LCD螢幕，顯示出一個交錯的ST LOGO


## Reference

- WAF 野生玩家 [可以看看](https://github.com/leemars/waf-learning)