<!--
 * @Author: SpenserCai
 * @Date: 2023-07-28 14:35:35
 * @version: 
 * @LastEditors: SpenserCai
 * @LastEditTime: 2023-08-03 23:57:02
 * @Description: file content
-->
# DeOldify for Stable Diffusion WebUI
This is an extension for StableDiffusion's [AUTOMATIC1111 web-ui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) that allows colorize of old photos. It is based on [deoldify](https://github.com/jantic/DeOldify).

![example](examples/demo.jpeg)

## Compatibility

### OS

<!--制作一个表格显示操作系统的兼容性，Windows不确定，linux兼容-->
| OS | Compatibility |
| :----: | :----: |
| Windows | ❓ |
| Linux | ✅ |


### Pytorch
<!--制作一个表格显示Pytorch版本的兼容性-->
| Version | Compatibility | Remark |
| :----: | :----: | :----: |
| <=1.13.1+cu117 | ✅ | |
| 2.1.0.dev20230711+rocm5.5  | ✅ | Thanks for [@fgtm2023](https://github.com/fgtm2023) test | 

### Other
If you have tested other systems or Pytorch during use, please submit a PR and attach a screenshot of the successful operation. Thank you

## Installation
In web-ui, go to the "Extensions" tab and use this URL https://github.com/SpenserCai/sd-webui-deoldify in the "install from URL" tab.

## Usage
1.To completely exit webui, you need to add `--disable-safe-unpickle` at startup.

2.In web-ui, go to the "Extra" tab and select "DeOldify" checkbox.

3.Upload the old photo you want to colorize.

## Application Scenario
Combining Upscale, GFPGAN, and Denoldify for old photo restoration effects

| Before | After |
| :----: | :----: |
| <img src="examples/before.jpeg" alt="before" align=center /> | <img src="examples/after.jpeg" alt="after" align=center /> |

## TODO
- [ ] Support video colorization
- [ ] Support repair options
- [ ] Support for simultaneous generation of images with different Render Factor values and Artistic on/off like “X/Y/Z Script” [#2](https://github.com/SpenserCai/sd-webui-deoldify/issues/2)



