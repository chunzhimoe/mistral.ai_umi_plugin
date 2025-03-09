# Mistral OCR 插件

这是一个基于Mistral AI OCR API的Umi-OCR插件，可以帮助您使用Mistral的OCR服务进行文字识别。

## 安装说明

1. 将整个`MistralOCR`文件夹放入Umi-OCR的插件目录：`UmiOCR-data\plugins\`

2. 重启Umi-OCR

> **注意**: 插件已内置所有必要的依赖库，无需手动安装任何依赖。

## 配置说明

### 全局配置
- **API密钥**: 您的Mistral API密钥，可以从[Mistral AI控制台](https://console.mistral.ai/)获取
- **模型**: OCR模型名称，默认为`mistral-ocr-latest`
- **超时时间**: API请求的超时时间（秒）
- **包含图像Base64**: 是否在响应中包含图像的Base64编码（高级选项）

### 局部配置
- **语言**: 识别的目标语言，支持自动检测、中文、英文等多种语言
- **最小图像尺寸**: 提取图像的最小尺寸（像素），0表示不限制（高级选项）

## 使用方法

1. 启动Umi-OCR后，在全局设置中切换到"Mistral OCR"
2. 配置您的API密钥和其他参数
3. 在识别界面选择"文字识别（Mistral OCR）"
4. 设置识别语言等参数
5. 开始使用OCR功能

## 故障排除

如果遇到OCR识别失败，请检查：

1. 您的API密钥是否正确配置
2. 网络连接是否正常
3. 您的Mistral账户是否有足够的额度

## 注意事项

- 使用此插件需要有效的Mistral API密钥
- OCR识别会消耗您的Mistral API额度
- 请确保您的网络环境能够访问Mistral API服务器
