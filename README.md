# wxworkhook

wxworkhook 是一款基于 Windows PC 端企业微信的 Hook 工具，将企微常用功能封装为丰富稳定的 HTTP 接口，开箱即用，方便开发者快速接入、自由扩展，非常适合自动化脚本与二次开发场景。

## 使用说明

直接 clone 到本地，命令行执行：

```bash
.\NoveHost64.exe --port 5001 --receive-url "http://127.0.0.1:9000/wecom/event"
```

- `--port`：API 调用端口
- `--receive-url`：消息接收地址，DLL 会主动推送消息到此地址

## 特别说明

> 开源版仅支持发送文本，且不支持长时间运行。

## 文本发送接口

```
POST http://127.0.0.1:port/api/send_text
```

请求 JSON 示例：

```json
{
    "type": 10266,
    "conversation_id": "R:10955919327227306",
    "content": "你好，888"
}
```

## 技术支持

QQ：`3628048254`（备注来意）

## 声明

本项目仅供技术研究，请勿用于非法用途。如有任何人凭此做何非法事情，均与作者无关，特此声明。
